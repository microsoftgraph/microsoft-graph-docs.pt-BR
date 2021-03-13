---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 105e201a0d28c20478213eb05906aab0c1fd59af
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780064"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let availableProviderTypes = await client.api('/identityProviders/availableProviderTypes')
    .version('beta')
    .get();

```