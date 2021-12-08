---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08dd489fd7f122c22c4e889bc72acb33ab6772a0
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346645"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackages = await client.api('/identityGovernance/entitlementManagement/accessPackages')
    .get();

```