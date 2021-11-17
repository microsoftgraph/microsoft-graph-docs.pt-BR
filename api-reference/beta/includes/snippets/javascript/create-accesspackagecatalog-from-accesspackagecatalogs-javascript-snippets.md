---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 825e7bf3105417ae9472fc50c045a95379ee10daff592ffb7d206b384b9e13a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156587"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageCatalog = {
  displayName: 'sales',
  description: 'for employees working with sales and outside sales partners',
  isExternallyVisible: true
};

await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs')
    .version('beta')
    .post(accessPackageCatalog);

```