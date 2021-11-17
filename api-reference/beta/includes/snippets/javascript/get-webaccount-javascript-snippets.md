---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c73ab2dc9aa1b0601ff03abd741d6dcc13e65277491250c3a07f5a25f0bfb7eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let webAccount = await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .get();

```