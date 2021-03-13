---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94b9eb0e059216b17caf545b24a30f091c479537
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let used = await client.api('/me/insights/used')
    .version('beta')
    .get();

```