---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd284347307d229e74ecb839c7d646b1328e398f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783045"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/beta/education/users/13015'
};

await client.api('/education/classes/11011/members/$ref')
    .version('beta')
    .post(educationUser);

```