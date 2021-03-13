---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1237c6ed8fc02d84263d910c7cb340b711317dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator')
    .version('beta')
    .delete();

```