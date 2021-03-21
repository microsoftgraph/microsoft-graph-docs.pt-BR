---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39898afb54f3cbc0729fc3fd0c72a58bfab2f6b2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/contacts/{id}/manager')
    .version('beta')
    .get();

```