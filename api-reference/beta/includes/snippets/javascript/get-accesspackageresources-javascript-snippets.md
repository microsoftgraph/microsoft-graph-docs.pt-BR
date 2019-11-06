---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93a81ecb041551ddc1475ed13b4cff1b4cf9280f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources')
    .version('beta')
    .get();

```