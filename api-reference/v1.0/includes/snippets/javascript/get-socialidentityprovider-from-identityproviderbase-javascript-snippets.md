---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 854820d211257b649f2166d0a89c2d8f4522245c909664df9fac60defe8a3374
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407087"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/Amazon-OAUTH')
    .get();

```