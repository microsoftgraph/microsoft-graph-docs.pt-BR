---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c61910d71e9a5c81ef138a39383432a0434e9ba3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666643"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/users/{id | userPrincipalName}')
    .select('displayName,givenName,postalCode')
    .get();

```