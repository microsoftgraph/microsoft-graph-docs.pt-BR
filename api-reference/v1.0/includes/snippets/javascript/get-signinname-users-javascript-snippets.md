---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8fb0b16875ef8cb87b265a4cd3ceaed5cb71d96
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .filter('identities/any(c:c/issuerAssignedId eq \'j.smith@yahoo.com\' and c/issuer eq \'contoso.onmicrosoft.com\')')
    .select('displayName,id')
    .get();

```