---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7848c3422c29629de91ae11899c59bc41fba98ec
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/appRoleAssignments')
    .get();

```