---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43eb0f7cd1f5abd7bdfd80f23cb2bf0d8d219cbd
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deviceRegistrationPolicy = await client.api('/policies/deviceRegistrationPolicy')
    .version('beta')
    .get();

```