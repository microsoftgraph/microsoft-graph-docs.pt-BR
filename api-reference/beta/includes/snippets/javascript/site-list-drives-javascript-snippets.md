---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1f2e02e3fa637b9ab9abcf0127cb7a700eb91ce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/sites/{siteId}/drives')
    .version('beta')
    .get();

```