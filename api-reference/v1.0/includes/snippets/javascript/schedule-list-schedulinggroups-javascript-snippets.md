---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b684fdcfa4bbd803f5cb230211bd5c56fc16d7f0
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44218118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .get();

```