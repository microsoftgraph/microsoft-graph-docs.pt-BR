---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf1ac8f7786a1bb03dcb10860f7c4c49bd8b57eb00d923cdd45e52ecd1f80f1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf')
    .version('beta')
    .get();

```