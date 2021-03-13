---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2db9ca849d5379ef31ef8149ba3b0cf252c6f12
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let passwordMethods = await client.api('/me/authentication/passwordMethods')
    .version('beta')
    .get();

```