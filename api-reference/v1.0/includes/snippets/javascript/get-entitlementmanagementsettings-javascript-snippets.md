---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 770044bb31a19e02aae8fd7fc8399e991c2c2b8b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340074"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let entitlementManagementSettings = await client.api('/identityGovernance/entitlementManagement/settings')
    .get();

```