---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 693f414d7ceb7ff02ad9afcde06513f7b8edcb76c0ad6618e974bcd9bbed2869
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffRequest = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .version('beta')
    .get();

```