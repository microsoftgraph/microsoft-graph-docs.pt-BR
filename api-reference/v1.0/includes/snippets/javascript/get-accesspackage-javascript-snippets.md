---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5034d0cb27067b5fd1c37cbfa06d35b3a008cd17
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackage = await client.api('/identityGovernance/entitlementManagement/accessPackages/114d3459-3459-114d-5934-4d1159344d11')
    .get();

```