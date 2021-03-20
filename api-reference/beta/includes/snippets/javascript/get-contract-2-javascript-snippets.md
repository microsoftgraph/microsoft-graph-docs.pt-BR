---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 837d92897963551754cb579572856066c768f27a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contracts = await client.api('/contracts')
    .version('beta')
    .get();

```