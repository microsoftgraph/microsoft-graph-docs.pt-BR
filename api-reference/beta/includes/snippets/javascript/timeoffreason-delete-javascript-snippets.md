---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 941c1081550f875c4457f8a532679eee4ebe5e8e2b8ffcbb31297e5d0505a452
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100336"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .version('beta')
    .delete();

```