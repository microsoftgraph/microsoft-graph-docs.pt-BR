---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8b9a0ef992be0f62ed74d922e719ac44a8b90a7
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/phoneMethods')
    .version('beta')
    .get();

```