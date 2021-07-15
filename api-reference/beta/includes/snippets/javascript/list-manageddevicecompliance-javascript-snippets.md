---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9450f1fdeb69862da3681806cd2318d96fc6db6d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managedDeviceCompliances = await client.api('/tenantRelationships/managedTenants/managedDeviceCompliances')
    .version('beta')
    .get();

```