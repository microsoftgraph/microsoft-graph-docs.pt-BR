---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6fe68f6556f30647300a335f0a9acaf5cc8bfe11ab95293ec654e6bee682f74c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let swapShiftsChangeRequest = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}')
    .get();

```