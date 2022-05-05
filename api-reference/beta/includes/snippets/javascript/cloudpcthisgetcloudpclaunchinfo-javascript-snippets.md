---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39720b7c1bc78a24d76f20ef063a759c377e7f08
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcLaunchInfo = await client.api('/me/cloudPCs/{cloudPCId}/getCloudPcLaunchInfo')
    .version('beta')
    .get();

```