---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29c748cdf4c99ca19d31bcab665bc532f2d4685af69b4e10c4770c0a687df0dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156620"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let incompatibleGroups = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups')
    .version('beta')
    .get();

```