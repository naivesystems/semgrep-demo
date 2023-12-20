Run the commands below in the project root:

```
mkdir -p output

podman run --rm \
  -v $PWD:/src:O \
  -v $PWD/.naivesystems:/config:Z \
  -v $PWD/output:/output:Z \
  naive.systems/analyzer/misra:dev \
  /opt/naivesystems/misra_analyzer -show_results
```
