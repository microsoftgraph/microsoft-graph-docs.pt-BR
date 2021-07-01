---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23f80c02f0cc93b8b719d152e41d671320f9b42c
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53237076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser(on='target')')
    .version('beta')
    .get();

```