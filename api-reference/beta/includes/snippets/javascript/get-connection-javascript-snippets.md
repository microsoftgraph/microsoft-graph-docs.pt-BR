---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf1e30184fb1471476d339aa94c180fc0c586bc5
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectionQuota = await client.api('/external/connections/contosohr/quota')
    .version('beta')
    .get();

```