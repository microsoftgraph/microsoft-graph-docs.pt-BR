---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57a4374829e38812ee37f77155419b53b70b5b3a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}')
    .delete();

```