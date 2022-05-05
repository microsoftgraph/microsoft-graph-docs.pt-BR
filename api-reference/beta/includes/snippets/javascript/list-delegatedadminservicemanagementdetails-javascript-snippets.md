---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3872adbeba516696ebb36985073a62152fe07990
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceManagementDetails = await client.api('/tenantRelationships/delegatedAdminCustomers/4fdbff88-9d6b-42e0-9713-45c922ba8001/serviceManagementDetails')
    .version('beta')
    .get();

```