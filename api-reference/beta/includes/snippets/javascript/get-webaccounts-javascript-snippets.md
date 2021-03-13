---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1081961e31f51955cb98cf502315fc05d6c71e46
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805612"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let webAccounts = await client.api('/me/profile/webAccounts')
    .version('beta')
    .get();

```