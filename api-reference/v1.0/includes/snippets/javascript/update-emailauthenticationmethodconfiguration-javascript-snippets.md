---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0aaec0b6b93faa97d29a2885d2ca7707833eb2fa938a983dd50fbeabe3fbd2e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  '@odata.type': '#microsoft.graph.emailAuthenticationMethodConfiguration',
  allowExternalIdToUseEmailOtp: 'enabled',
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email')
    .update(authenticationMethodConfiguration);

```