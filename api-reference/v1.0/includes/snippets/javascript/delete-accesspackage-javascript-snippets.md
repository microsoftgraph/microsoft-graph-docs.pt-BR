---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b40870ac45b8efcf503ede04960802c0bf2f723b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}')
    .delete();

```