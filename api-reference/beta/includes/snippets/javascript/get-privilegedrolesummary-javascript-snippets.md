---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10a420e1fa82fae37837b8eafbc7cf03112003193a526fdb8d9d4d8fbe7cb41f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleSummary = await client.api('/privilegedRoles/{id}/summary')
    .version('beta')
    .get();

```