---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42bf00839b026f23fdd9de0b2f9d2b0371c39fef
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .delete();

```