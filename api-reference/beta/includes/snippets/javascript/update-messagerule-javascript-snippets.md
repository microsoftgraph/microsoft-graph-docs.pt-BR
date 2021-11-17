---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8181ce8fe1611a5351d73f4a4d1b4613c17bd0215c14eb56eee66ef185293830
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: 'Important from partner',
    actions: {
        markImportance: 'high'
     }
};

await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')')
    .version('beta')
    .update(messageRule);

```