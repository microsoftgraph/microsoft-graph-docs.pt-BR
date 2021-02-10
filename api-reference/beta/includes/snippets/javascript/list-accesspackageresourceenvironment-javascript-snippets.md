---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57fd8f13b94682c391fb6aa31c566744a483a4d3
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceEnvironments')
    .version('beta')
    .filter('originSystem eq 'SharePointOnline'')
    .get();

```