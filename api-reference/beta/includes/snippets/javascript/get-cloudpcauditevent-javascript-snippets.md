---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a56835fa6cad4a0d2be22796dd1689fc8737bdf5
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcAuditEvent = await client.api('/deviceManagement/virtualEndpoint/auditEvents/{id}')
    .version('beta')
    .get();

```