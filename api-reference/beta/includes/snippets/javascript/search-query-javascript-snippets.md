---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ef5db3a7cc6c5d8be24fa30f6f716c81285e649
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const searchResponse = {
  requests: [
    {
      entityTypes: [
        "externalItem"
      ],
      contentSources: [
        "/external/connections/connectionfriendlyname"
      ],
      query: {
        queryString: "contoso product"
      },
      from: 0,
      size: 25,
      fields: [
        "title",
        "description"
      ]
    }
  ]
};

let res = await client.api('/search/query')
    .version('beta')
    .post(searchResponse);

```