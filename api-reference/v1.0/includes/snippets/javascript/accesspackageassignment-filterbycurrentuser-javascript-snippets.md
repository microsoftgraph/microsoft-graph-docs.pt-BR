---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3ee8c7459bc0caf8fc3e337c84348161216bb6d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342872"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/assignments/filterByCurrentUser(on='target')')
    .get();

```