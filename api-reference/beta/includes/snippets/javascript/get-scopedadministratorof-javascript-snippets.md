---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 405b68e15f9171cdbc59d289c2f68f8113a114a54021497e7df2c6841098e259
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329546"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMemberOf = await client.api('/me/scopedRoleMemberOf')
    .version('beta')
    .get();

```