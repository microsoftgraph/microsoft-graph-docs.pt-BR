---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5d591796634d35749c6de15b0d801495e5a3a71
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref')
    .version('beta')
    .delete();

```