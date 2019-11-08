---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce5fe3c4b243505372b911946d00271ffe69ec0a
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2019
ms.locfileid: "38027100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/versions/{version-id}/content')
    .version('beta')
    .get();

```