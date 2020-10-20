---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f54fdda89d556fd0476b14f0a185b836da54f4bb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignments/{id}/makeEligible')
    .version('beta')
    .post();

```