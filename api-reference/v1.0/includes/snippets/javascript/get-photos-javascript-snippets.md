---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fae01e61308e86ba111bd67eac05cc4066609533
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let photos = await client.api('/groups/{id}/photos')
    .get();

```