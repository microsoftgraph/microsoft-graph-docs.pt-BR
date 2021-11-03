---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d1a06e55228f2766cd09381e9425e0bbb98eee4f72cfb0823ee740e762fce2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageCatalog = {
  displayName: 'Catalog One'
};

await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}')
    .version('beta')
    .update(accessPackageCatalog);

```