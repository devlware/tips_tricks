> Get the sum of all Persistent Volumes in your cluster.

```zsh
kubectl get pv --no-headers | awk -e '{print $2}' | cut -dG -f1  | awk '{s+=$1} END {print s}'
```


```zsh
for name in $(ls -d */ | tr -d '/' | egrep -v '(pattern1|pattern2)'); \
do
  cd $name; \
  hub pull-request -b develop -m "bump version to v1.5.2" -r gituser1,gituser2 -a gituser1,gituser2 -l "Priority: High";
  cd ..;
done
```
