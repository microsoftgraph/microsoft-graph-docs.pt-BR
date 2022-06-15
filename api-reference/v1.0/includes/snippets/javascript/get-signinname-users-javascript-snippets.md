---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f70d13a7b0c7ac4412a933e6f895c73ac726a79
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .filter('identities/any(c:c/issuerAssignedId eq \'j.smith@yahoo.com\' and c/issuer eq \'My B2C tenant\')')
    .select('displayName,id')
    .get();

```