---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 894975dbcc14a908df860a08902f9659008989b11ca3a1ff1414b57825daf91f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'message-value'
};

await client.api('/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve')
    .post(approve);

```