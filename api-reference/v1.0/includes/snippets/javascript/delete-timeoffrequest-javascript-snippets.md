---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c58727c8dba0b0f49faa476f1ac82ee4466491c138338408fab3a95796153d6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .delete();

```