---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dfeac0b84415e5de171cbef5b24adbd10526348e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805384"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScores = await client.api('/security/secureScores')
    .version('beta')
    .top(1)
    .get();

```