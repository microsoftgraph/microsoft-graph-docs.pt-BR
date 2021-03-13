---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4880287eb91f5c3e466fce4bf8c7cd26d9cce5ef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let microsoftAuthenticatorAuthenticationMethod = await client.api('/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2')
    .version('beta')
    .get();

```