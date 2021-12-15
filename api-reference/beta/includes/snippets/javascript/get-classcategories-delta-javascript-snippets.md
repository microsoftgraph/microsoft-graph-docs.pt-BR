---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d45f6f0f2d270013c32d7f66062c429c0defdad
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationCategory = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta')
    .version('beta')
    .get();

```