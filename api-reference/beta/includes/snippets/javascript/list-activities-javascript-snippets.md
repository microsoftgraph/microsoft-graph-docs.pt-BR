---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1cb794d308b82f6bbe1df37c3e417e4b5947e5e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activities = await client.api('/me/drive/activities')
    .version('beta')
    .get();

```