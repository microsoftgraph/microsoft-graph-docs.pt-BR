---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d9e1adda2d3e4796cfadf5cbd66fb77b376d2be6833a75a0c5ee5099035262e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216868"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const projectParticipation = {
  allowedAudiences: 'organization',
  client: {
    department: 'Corporate Marketing',
    webUrl: 'https://www.contoso.com'
  }
};

await client.api('/me/profile/projects/{id}')
    .version('beta')
    .update(projectParticipation);

```