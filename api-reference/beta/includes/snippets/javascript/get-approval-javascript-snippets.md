---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb127930995594dd96406416b32e442f8967e7454903cb75816e1fddd4db0132
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let approval = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489')
    .version('beta')
    .get();

```