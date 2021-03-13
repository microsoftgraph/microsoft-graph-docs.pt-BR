---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1064ba2748f7009cc293964834c34bc1002ca1b5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notes = await client.api('/me/profile/notes')
    .version('beta')
    .get();

```