---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 184f233437ff6e9c3c38e807ec0e10986fd1c503
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/4aade2547798441eab5188a7a2436bc1/$value')
    .version('beta')
    .get();

```