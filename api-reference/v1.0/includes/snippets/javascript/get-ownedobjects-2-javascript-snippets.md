---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afd9cc777687977fd526f771ffee0a96072f0a48
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/me/ownedObjects')
    .get();

```