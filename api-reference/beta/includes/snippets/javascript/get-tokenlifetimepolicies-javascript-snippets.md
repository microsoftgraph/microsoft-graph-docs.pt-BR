---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f646e33ee2d18b535652794a211d943bbcb8fa7e
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558913"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenLifetimePolicies')
    .version('beta')
    .get();

```