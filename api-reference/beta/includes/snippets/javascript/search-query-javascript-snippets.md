---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9cc43ad25eb51a8180787497e8a9fcf0ae667863724b7035d686dbe439c7ef67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214519"
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
        'externalItem'
      ],
      contentSources: [
        '/external/connections/connectionfriendlyname'
      ],
      query: {
        queryString: 'contoso product'
      },
      from: 0,
      size: 25,
      fields: [
        'title',
        'description'
      ]
    }
  ]
};

await client.api('/search/query')
    .version('beta')
    .post(searchResponse);

```