---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8fdef1eb31db0c284ba911ecffc101ece9de035
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref')
    .version('beta')
    .delete();

```