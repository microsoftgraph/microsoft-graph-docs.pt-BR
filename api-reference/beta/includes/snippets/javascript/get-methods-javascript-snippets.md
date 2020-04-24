---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78e47fe1eb6fb4bff38559784f8e35b599a510ae
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/methods')
    .version('beta')
    .get();

```