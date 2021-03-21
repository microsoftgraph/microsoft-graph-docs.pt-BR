---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb9b5e129214015b0b2a1b5f0aae5149aac1b4f2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contract = await client.api('/contracts/{id}')
    .get();

```