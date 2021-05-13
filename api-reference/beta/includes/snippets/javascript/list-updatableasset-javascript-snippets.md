---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 872fc80e86801ebdd5546bfbdf69e65f06dc0f1a
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52476803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let exclusions = await client.api('/admin/windows/updates/deployments/{deploymentId}/audience/exclusions')
    .version('beta')
    .get();

```