---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4861227886856fee57fe0b79ff6ab4da06829ee
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/getMemberGroups')
    .post(string);

```