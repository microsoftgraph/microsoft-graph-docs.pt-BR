---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b855487215f2205a9fa33ac4a8289d6ee03e747e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953992"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass')
    .version('beta')
    .delete();

```