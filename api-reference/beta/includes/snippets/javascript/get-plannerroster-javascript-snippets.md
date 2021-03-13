---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9891f33d8625d6f256221981300462614d980a50
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795670"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerRoster = await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965')
    .version('beta')
    .get();

```