---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edea9c5f3615255caa8c04adc0b7024bb1043669
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userPurpose = await client.api('/me/mailboxSettings/userPurpose')
    .version('beta')
    .get();

```