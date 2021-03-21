---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 630cebaa97465d9c095f44fa221af56ec95288e1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contracts = await client.api('/contracts')
    .get();

```