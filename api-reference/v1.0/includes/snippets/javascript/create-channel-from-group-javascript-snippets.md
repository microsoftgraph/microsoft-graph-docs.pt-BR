---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9baee5663c32ba934ae21a4403fe7498245bb364
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465301"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: "Architecture Discussion",
  description: "This channel is where we debate all future architecture plans"
};

let res = await client.api('/teams/{id}/channels')
    .post({channel : channel});

```