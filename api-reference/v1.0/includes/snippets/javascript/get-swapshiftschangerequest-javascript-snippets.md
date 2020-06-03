---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 873fe67510dabce2ad1d63e64776d2b514feea85
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests')
    .get();

```