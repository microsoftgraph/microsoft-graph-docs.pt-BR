---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8169e52ccdde30c7ee07af046236b6243288e0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffReasons = await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .get();

```