---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da2414ec62fc8a4752e33c4d810e5da965a99d58
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}')
    .version('beta')
    .get();

```