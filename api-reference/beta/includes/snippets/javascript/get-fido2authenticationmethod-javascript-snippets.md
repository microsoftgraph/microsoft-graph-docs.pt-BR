---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c606428967ea24dfb860b4ea09492a1f745d1d2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let fido2Methods = await client.api('/me/authentication/fido2Methods')
    .version('beta')
    .get();

```