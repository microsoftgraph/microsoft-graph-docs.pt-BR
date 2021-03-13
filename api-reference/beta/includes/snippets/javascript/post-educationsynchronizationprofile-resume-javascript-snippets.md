---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 457deb896c2bc2158fc814c8f7b9e42aa73717e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}/resume')
    .version('beta')
    .post();

```