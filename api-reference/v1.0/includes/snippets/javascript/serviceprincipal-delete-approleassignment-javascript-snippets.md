---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a51a222921a040fb0f9dc22b1f07e346ee2a1807
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/appRoleAssignments/{id}')
    .delete();

```