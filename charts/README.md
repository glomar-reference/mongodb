# Smoketest

helm upgrade \
  --create-namespace \
  --install \
  --wait \
  --namespace=open5gs \
  "mongodb" \
  "$(git rev-parse --show-toplevel)/charts/mongodb"