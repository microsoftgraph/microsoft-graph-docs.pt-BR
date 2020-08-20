---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc7ae31c13b00d23db18dcc931ceba623e8cca9b
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819432"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/phones')
    .version('beta')
    .get();

```