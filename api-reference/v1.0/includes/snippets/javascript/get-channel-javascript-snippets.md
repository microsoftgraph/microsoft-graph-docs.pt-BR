---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2865c9392cc854d045f5ff12a48c1c71825c2768
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channel = await client.api('/teams/{id}/channels/{id}')
    .get();

```