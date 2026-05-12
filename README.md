name: V2Ray_Server_6h
on: [workflow_dispatch]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Install V2Ray
        run: |
          bash <(curl -L https://raw.githubusercontent.com/v2fly/fscript/master/fscript.sh)
          sleep 21600 # Garde le serveur actif 6 heures (21600 secondes)

