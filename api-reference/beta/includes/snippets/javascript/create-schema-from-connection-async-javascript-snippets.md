---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c43b438b60ff0ace9de2ac5298f30c87139deea
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37995476"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schema = {
  baseType: "microsoft.graph.externalItem",
  properties: [
    {
      name: "title",
      type: "String",
      isSearchable: "true",
      isRetrievable: "true"
    },
    {
      name: "priority",
      type: "String",
      isQueryable: "true",
      isRetrievable: "true"
    },
    {
      name: "assignee",
      type: "String",
      isRetrievable: "true"
    }
  ]
};

let res = await client.api('/connections/contosohr/schema')
    .version('beta')
    .post(schema);

```