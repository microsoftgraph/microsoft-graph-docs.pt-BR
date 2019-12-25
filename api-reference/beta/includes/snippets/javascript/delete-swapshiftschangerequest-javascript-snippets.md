---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3149d92c04b45940dc69dcf2b181264574bd89a4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870847"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/schedule/swapShiftsChangeRequests')
    .version('beta')
    .delete();

```