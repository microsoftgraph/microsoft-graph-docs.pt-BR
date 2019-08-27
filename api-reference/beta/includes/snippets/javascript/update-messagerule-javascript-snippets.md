---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc70d790eb28b11563898bf1b23fc7ba8de04ce3
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636300"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: "Important from partner",
    actions: {
        markImportance: "high"
     }
};

let res = await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')')
    .version('beta')
    .update(messageRule);

```