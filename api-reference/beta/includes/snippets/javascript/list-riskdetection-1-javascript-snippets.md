---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d97f025e08690fc84c9b28687d1e8ebc033220e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetections = await client.api('/riskDetections')
    .version('beta')
    .get();

```