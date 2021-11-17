---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7354be31802f447cffc0e17de1f47f59218108a64320f0d57888b0d357cc8903
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .delete();

```