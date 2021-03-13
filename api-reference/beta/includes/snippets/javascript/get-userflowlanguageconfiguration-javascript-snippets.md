---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41ae983a142763fa97a782113746d7a28bd3151f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789636"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages')
    .version('beta')
    .get();

```