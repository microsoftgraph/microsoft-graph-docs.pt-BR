---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46d707cdb9453d025bf975afa03d43993bbfcaab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801645"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffRequest = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .get();

```