---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7ed05ec0c9eebeffa8d3f860937cbacee046cae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779330"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let joinedTeams = await client.api('/me/joinedTeams')
    .get();

```