---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 325b710da0bb70b48fcb9419990f584cf620cce8fdb1859b296a926b22c96937
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899096"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicyAssignments = await client.api('/policies/roleManagementPolicyAssignments')
    .version('beta')
    .get();

```