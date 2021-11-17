---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 031e65ee4a155b2e4265497e894d96dde4fdba31325f7d88749aae20e5e7ff93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .version('beta')
    .delete();

```