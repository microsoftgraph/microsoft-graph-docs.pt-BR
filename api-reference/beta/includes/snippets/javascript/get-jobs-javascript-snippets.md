---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62073207a31f5aca5762c032d97c693364384a9e
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015655"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/jobs')
    .version('beta')
    .get();

```