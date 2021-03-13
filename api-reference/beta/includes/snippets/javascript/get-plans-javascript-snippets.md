---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 641d3448804e988a52da59adb91907bac0246253
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779605"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/planner/plans')
    .version('beta')
    .get();

```