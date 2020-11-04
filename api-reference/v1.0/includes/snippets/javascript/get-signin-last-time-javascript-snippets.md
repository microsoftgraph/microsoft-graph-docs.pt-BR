---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f39a847d9fb5f638a0847c367ebef37b326a960f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .select('displayName,userPrincipalName,signInActivity')
    .get();

```