---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d002d4d270d5b859d018dd2eecf65de661d50d17cb91b18b5a2f9e2f21c461f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215256"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let includes = await client.api('/policies/permissionGrantPolicies/microsoft-application-admin/includes')
    .get();

```