---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8908a7d62bea787c3262a05fdab514f10ad09eb74e7101e13cfc461aab35917d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .version('beta')
    .delete();

```