---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41e6a5cffc792f85ab494ebaa903b29bbace0a3f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789678"
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