---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7cfec7b5b7204457bde0cb2d1948bacdfa8cdbb
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524330"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy')
    .delete();

```