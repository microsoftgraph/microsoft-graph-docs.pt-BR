---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9dc89df34ca0fffa3c3293518387fc72665eb828
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .get();

```