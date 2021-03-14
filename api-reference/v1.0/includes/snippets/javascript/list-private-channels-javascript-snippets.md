---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1055a61a0a89a3d7fa0e22eeb316e5576aa7578b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799128"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/{id}/channels')
    .version('beta')
    .filter('membershipType eq \'private\'')
    .get();

```