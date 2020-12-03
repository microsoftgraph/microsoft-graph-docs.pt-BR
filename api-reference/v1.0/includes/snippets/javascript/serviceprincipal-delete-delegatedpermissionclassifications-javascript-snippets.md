---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9dd839f1b85871a47f30f377fa5ab09657624f0
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications/{id}')
    .delete();

```