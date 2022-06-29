---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4855bd052d83fea4963f35d505741720771b3b71
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  '@odata.type':'#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration',
  isUsableOnce: true
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/temporaryAccessPass')
    .version('beta')
    .update(authenticationMethodConfiguration);

```