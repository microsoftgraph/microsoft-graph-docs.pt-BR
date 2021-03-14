---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0e8575ab09c9db470754096eb0a0bc5e18f77f3b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOff = await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .get();

```