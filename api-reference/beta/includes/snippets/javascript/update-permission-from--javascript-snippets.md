---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6fb22810142a4e7d7c3d14d2e4a0aa23fe5d368764c24669b948f03653d93289
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328009"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: ['read']
};

await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .update(permission);

```