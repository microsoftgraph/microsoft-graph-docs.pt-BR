---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f027ba5825de734add5d3d593583a626ca21dc81
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/groups/{id}/members')
    .get();

```