---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dafd7937fc9f54d94be084087f4c4a3776815792
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015934"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11014/schools')
    .version('beta')
    .get();

```