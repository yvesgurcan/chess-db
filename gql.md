query getFile {

  repository(name: "chess-db", owner: "yvesgurcan") {
    object(expression: "master:README.md") {
      ... on Blob {
        text
      }
    }
  }
}

