---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63602eac1147a577b7de4ea069dfa814e920251ce8e6a7a456bb59eb1950f90b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213910"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve')
    .post(approve);

```