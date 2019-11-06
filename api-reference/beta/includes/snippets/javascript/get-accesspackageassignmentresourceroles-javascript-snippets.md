---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1487c552cc9a587c1d6dca0498b3a3d37b30f8f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles')
    .version('beta')
    .get();

```