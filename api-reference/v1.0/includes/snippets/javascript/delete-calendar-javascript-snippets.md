---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7341a3ebc0b6d340199d18287a1d248b55897743
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/calendar')
    .delete();

```