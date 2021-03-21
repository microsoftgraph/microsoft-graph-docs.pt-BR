---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfdcdd3d404ce4b517a3b12f432fea54333e4f0c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let settings = await client.api('/me/analytics/settings')
    .version('beta')
    .get();

```