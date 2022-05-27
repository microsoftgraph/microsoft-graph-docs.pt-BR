---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb28d1813fc834d24d1fca7089a2759ea731dec451abf0395c0942bacfd30d65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref')
    .version('beta')
    .delete();

```