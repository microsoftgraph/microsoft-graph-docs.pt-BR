---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f638a829c6becb9b0bd2c6ca4de8ac1c8ea17bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791525"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let used = await client.api('/me/insights/used')
    .get();

```