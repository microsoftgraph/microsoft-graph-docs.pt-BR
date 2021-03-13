---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e3b3f18f0d48273de85d7bb9f3966db4338842d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803345"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemPublication = await client.api('/me/profile/publications/{id}')
    .version('beta')
    .get();

```