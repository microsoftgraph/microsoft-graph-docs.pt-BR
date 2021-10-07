---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1566fb2cd658d249e432fae385e1614cc2cbe52a2ccc624442e8fe9fdf1a127
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327823"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  '@odata.type': '#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration',
  state: 'String'
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .version('beta')
    .update(authenticationMethodConfiguration);

```