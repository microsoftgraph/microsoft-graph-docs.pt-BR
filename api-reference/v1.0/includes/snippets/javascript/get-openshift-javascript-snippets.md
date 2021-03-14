---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d71c4fdff038ae4074ed6940790462cbe756063b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShifts = await client.api('/teams/{id}/schedule/openShifts')
    .get();

```