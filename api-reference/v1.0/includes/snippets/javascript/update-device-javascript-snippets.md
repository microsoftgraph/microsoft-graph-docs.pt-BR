---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b5c6a09bdef7d791795216313b7da6a1d4fee1f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false
};

let res = await client.api('/devices/{id}')
    .update(device);

```