---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4671aefdd74def66348ce0c80917c03addc11a9cf1987f3d1822d96137f8b65c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cAuthenticationMethodsPolicy = await client.api('/policies/b2cAuthenticationMethodsPolicy')
    .version('beta')
    .get();

```