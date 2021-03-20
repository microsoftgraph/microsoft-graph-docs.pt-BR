---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a34c0e51eac2501188de0f994ea6bf58da5b4096
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/me/planner/plans')
    .get();

```