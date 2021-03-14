---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3870eb7da00c14f0e54f0a9add785deb909142fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityBasedTimeoutPolicy = await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .get();

```