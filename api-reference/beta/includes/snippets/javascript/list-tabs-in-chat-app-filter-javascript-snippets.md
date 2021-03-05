---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37acb7457d6618c96366c1c5371e7143a7312c82
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .version('beta')
    .filter('teamsApp/id eq \'com.microsoft.teamspace.tab.web\'')
    .expand('teamsApp')
    .get();

```