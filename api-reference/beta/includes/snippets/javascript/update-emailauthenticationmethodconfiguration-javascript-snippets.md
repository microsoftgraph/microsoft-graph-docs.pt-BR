---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38dda2920ad546d68917325eb8223708ec713b721d4bcdbbe8b197a6ae2f1b3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  '@odata.type': '#microsoft.graph.emailAuthenticationMethodConfiguration',
  allowExternalIdToUseEmailOtp: 'disabled',
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email')
    .version('beta')
    .update(authenticationMethodConfiguration);

```