---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f765955a4fd0dac2977a816e8aa87fbb9378c4d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}/replies')
    .version('beta')
    .get();

```