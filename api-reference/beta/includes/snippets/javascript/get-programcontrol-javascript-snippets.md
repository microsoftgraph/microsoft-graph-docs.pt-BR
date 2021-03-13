---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb8c288aa4fcb44dd9b7a0950b304d9fa398629c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let programControls = await client.api('/programControls')
    .version('beta')
    .get();

```