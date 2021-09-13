---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea23922bc7a7586350807bf96d2f9268739d09c8a72ebf830a39912e6fd35c9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffRequest = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .get();

```