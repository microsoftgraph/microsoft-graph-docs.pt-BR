---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e9d5fbd4d5b152a064e5cc9172847173a090ab4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/reports/getM365AppPlatformUserCounts(period='D7')/content')
    .version('beta')
    .get();

```