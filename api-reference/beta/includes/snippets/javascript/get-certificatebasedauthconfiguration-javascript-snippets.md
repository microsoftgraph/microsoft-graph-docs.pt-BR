---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31a6883e02398e368bdaaa9771a848dd4effe79d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let certificateBasedAuthConfiguration = await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .version('beta')
    .get();

```