---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e53297369d78232cb4fe926b988976480d63dacd
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notes = await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes')
    .version('beta')
    .get();

```