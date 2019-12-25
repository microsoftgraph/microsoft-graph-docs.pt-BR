---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d85222308cb7f02abd57a2c2c4adea25e89379a6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/appRoleAssignedTo/{id}')
    .version('beta')
    .delete();

```