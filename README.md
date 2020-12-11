# tekton 1

#https://developer.github.com/v3/repos/statuses/#create-a-commit-status

```
curl -X POST -H "Accept: application/vnd.github.v3+json" https://${gitApiKey}@api.github.com/repos/ajgarozz/tekton/statuses/${commitid} -d '{"state":"pending", "context":"this"}'
curl -X POST -H "Accept: application/vnd.github.v3+json" https://${gitApiKey}@api.github.com/repos/ajgarozz/tekton/statuses/${commitid} -d '{"state":"pending", "context":"is"}'
curl -X POST -H "Accept: application/vnd.github.v3+json" https://${gitApiKey}@api.github.com/repos/ajgarozz/tekton/statuses/${commitid} -d '{"state":"pending", "context":"an"}'
curl -X POST -H "Accept: application/vnd.github.v3+json" https://${gitApiKey}@api.github.com/repos/ajgarozz/tekton/statuses/${commitid} -d '{"state":"pending", "context":"example"}'

sleep 5

curl -X POST -H "Accept: application/vnd.github.v3+json" https://${gitApiKey}@api.github.com/repos/ajgarozz/tekton/statuses/${commitid} -d '{"state":"success", "context":"this", "target_url":"http://somepath.goes.here"}'
curl -X POST -H "Accept: application/vnd.github.v3+json" https://${gitApiKey}@api.github.com/repos/ajgarozz/tekton/statuses/${commitid} -d '{"state":"success", "context":"is", "target_url":"http://somepath.goes.here"}'
curl -X POST -H "Accept: application/vnd.github.v3+json" https://${gitApiKey}@api.github.com/repos/ajgarozz/tekton/statuses/${commitid} -d '{"state":"success", "context":"an", "target_url":"http://somepath.goes.here"}'
curl -X POST -H "Accept: application/vnd.github.v3+json" https://${gitApiKey}@api.github.com/repos/ajgarozz/tekton/statuses/${commitid} -d '{"state":"failure", "context":"example", "target_url":"http://somepath.goes.here"}'
```
