---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ec10aecd09a859a49b37ea820b6660e185ec7dc
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51572995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const associateWithHubSites = {
   hubSiteUrls: [
      'https://graph.microsoft.com/beta/sites/id'
   ],
   propagateToExistingLists: false
};

await client.api('/sites/id/contentTypes/id/associateWithHubSites')
    .version('beta')
    .post(associateWithHubSites);

```