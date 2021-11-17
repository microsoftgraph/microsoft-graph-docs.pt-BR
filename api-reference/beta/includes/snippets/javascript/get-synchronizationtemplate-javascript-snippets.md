---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 177f7c628820a8c85606ca422189e99f7f4bdf5833c9d22d091fba2e9d0ab9ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099610"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let templates = await client.api('/servicePrincipals/{id}/synchronization/templates')
    .version('beta')
    .get();

```