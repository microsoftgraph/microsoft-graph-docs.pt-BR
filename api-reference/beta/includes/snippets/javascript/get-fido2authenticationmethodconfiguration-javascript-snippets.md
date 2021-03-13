---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c02b658cc99ceaf35042f6828c381077d23adffc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809495"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .version('beta')
    .get();

```