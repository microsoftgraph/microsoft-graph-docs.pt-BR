---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70820f9ea7add4fd138908f8bc29697e17b25e04
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957605"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookTask = await client.api('/me/outlook/tasks/AAMkADA1MTrgAAA=')
    .version('beta')
    .get();

```