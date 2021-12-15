---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23e6b64d21a3c9b687684c2a060eee5293d1ee7d
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const resizeCloudPc = {
  targetServicePlanId: '30d0e128-de93-41dc-89ec-33d84bb662a0'
};

await client.api('/deviceManagement/managedDevices/{managedDeviceId}/resizeCloudPc')
    .version('beta')
    .post(resizeCloudPc);

```