---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dfbb1d9c0cd3c9de6e59215dccd3c48a9af3849c
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513165"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/getMemberObjects')
    .version('beta')
    .post(string);

```