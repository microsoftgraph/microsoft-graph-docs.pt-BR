---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b66e26d0825fb0aec8c9c66768cfd396b19f917
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59508060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/managedDevices/{managedDeviceId}/resizeCloudPc')
    .version('beta')
    .post();

```