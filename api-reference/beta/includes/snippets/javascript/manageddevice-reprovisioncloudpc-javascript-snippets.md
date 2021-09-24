---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a0226f1eb02ecf2190239eba54a725be855c1e1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59508677"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/managedDevices/{managedDeviceId}/reprovisionCloudPc')
    .version('beta')
    .post();

```