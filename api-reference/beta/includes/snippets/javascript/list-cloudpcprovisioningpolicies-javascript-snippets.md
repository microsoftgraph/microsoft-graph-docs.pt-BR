---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6123102d7052f917ed3668880c3e8af56a1c33d272dd569fcd5611ded80db5ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let provisioningPolicies = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies')
    .version('beta')
    .get();

```