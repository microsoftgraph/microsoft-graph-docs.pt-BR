---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f784a4804724be16e9d4819411bc829107f82df
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821191"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const projectParticipation = {
  allowedAudiences: "organization",
  client: {
    department: "Corporate Marketing",
    webUrl: "https://www.contoso.com"
  }
};

let res = await client.api('/me/profile/projects/{id}')
    .version('beta')
    .update(projectParticipation);

```