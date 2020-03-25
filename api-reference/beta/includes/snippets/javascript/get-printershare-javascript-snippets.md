---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3094d72c0459d3fce9237daae1e4b0d6b700e225
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printerShares/{id}')
    .version('beta')
    .get();

```