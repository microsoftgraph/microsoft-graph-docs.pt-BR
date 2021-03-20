---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41e6a5cffc792f85ab494ebaa903b29bbace0a3f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896')
    .version('beta')
    .delete();

```