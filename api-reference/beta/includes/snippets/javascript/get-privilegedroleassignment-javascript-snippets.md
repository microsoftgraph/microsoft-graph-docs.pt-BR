---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3078fd1d147deda4b0788baa6c40681fab949b1623f945e4b39697e3d17aa9da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleAssignment = await client.api('/privilegedRoleAssignments/{id}')
    .version('beta')
    .get();

```