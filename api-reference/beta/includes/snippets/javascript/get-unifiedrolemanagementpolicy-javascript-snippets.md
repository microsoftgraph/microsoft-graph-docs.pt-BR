---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a428076c48a71ed419d2c3ca661712d8b00ecd7d0decbe1751bd8491aea532c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleManagementPolicy = await client.api('/policies/roleManagementPolicies/f93a5c37-5c37-f93a-375c-3af9375c3af9')
    .version('beta')
    .get();

```