---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5595a128b9d337243ddd0b03f4bdeccb1fcc5344db0772d69aa675ec445bedd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/appRoleAssignments/{id}')
    .version('beta')
    .delete();

```