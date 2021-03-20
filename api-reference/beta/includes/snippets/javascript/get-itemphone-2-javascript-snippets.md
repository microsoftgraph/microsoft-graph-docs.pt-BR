---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9bfbc6b32bf01de820901697eba25309de141299
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let phones = await client.api('/me/profile/phones')
    .version('beta')
    .get();

```