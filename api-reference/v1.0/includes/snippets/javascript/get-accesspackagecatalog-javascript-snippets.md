---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c776a9e25e2460ae493191fcafe9060c5dd169c8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335622"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageCatalog = await client.api('/identityGovernance/entitlementManagement/catalogs/b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1')
    .get();

```