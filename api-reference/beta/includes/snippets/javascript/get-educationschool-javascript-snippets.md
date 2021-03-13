---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b683e657db7f59617e0d7f6ccdbeb0d81f7da5b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSchool = await client.api('/education/schools/10001')
    .version('beta')
    .get();

```