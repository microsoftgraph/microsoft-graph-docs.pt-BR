---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61ec67eb1edd224889800557a20b50e978bd1482
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433370"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods')
    .version('beta')
    .get();

```