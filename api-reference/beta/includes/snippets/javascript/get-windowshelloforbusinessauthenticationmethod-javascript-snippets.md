---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afc1f7dde03d323a86bd47858da47068b64f4d5b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsHelloForBusinessAuthenticationMethod = await client.api('/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2')
    .version('beta')
    .get();

```