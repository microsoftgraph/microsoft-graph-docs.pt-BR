---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6dfad82da046cd76653300aec4fe90ddf2e3e75fba123a55e19156cd8511cf6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups')
    .version('beta')
    .post();

```