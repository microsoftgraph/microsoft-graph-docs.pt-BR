---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9ad9cd333516649dd5c2a5e53fc0bc958771c9cd41eb0b64d89b0c09e5f7327
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .version('beta')
    .delete();

```