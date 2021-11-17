---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa9b285a766c32ad54cdeb2659a6bd29407eedd295d746a0ae03af4826819ac9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentResourceRoles = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles')
    .version('beta')
    .get();

```