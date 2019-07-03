---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b86a51f5011660b609ea853b58eb49bce2cb13e8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492126"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{groupId}/drive')
    .get();

```