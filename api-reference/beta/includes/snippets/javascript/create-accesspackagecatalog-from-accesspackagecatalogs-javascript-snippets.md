---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57b392408a8d114564ee04ff10b9451167dcc883
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802323"
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