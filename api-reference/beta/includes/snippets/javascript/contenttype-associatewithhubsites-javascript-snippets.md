---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c345faad091fbf09a2741fe863df52476ca909cc
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
   hubSiteUrls: [
      'https://graph.microsoft.com/beta/sites/id'
   ],
   propagateToExistingLists: false
};

await client.api('/sites/id/contentTypes/id/associateWithHubSites')
    .version('beta')
    .post(contentType);

```