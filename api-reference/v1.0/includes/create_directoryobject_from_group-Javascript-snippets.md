---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b261ac6554656669f8dac5511a9aaf45a42892a2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/users/{id}"
};

let res = await client.api('/users/{id}/manager/$ref')
    .put({directoryObject : directoryObject});

```