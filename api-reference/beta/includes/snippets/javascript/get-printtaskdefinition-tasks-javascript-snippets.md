---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcfb8b4fe7c3bea8da43140c990eac83a9a46b5a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565165"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/taskDefinitions/92d72a3d-cad7-4809-8924-43833282b079/tasks')
    .version('beta')
    .get();

```