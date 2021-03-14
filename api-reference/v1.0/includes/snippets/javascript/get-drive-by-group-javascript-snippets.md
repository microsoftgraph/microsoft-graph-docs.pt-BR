---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d30ad0c73dab71b4f44ebca145f7680e1768bb9c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798330"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/groups/{groupId}/drive')
    .get();

```