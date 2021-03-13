---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f9147701a7421f5e1534b24b30ad72badfb5afb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796605"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let excludes = await client.api('/policies/permissionGrantPolicies/microsoft-application-admin/excludes')
    .version('beta')
    .get();

```