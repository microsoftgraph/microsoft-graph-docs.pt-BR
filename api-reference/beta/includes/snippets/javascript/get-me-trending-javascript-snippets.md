---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b66c0d7453a71914978dd6934c8f80008aee27d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let trending = await client.api('/me/insights/trending')
    .version('beta')
    .get();

```