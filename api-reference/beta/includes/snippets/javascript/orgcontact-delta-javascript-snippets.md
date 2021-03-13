---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29b7d959c51e96b4aec534a3ffcbbc36edda0cef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .version('beta')
    .get();

```