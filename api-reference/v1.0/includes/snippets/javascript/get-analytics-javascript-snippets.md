---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e90e5fb98d8989be08377cfd430b82cc6c7f4722
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/analytics')
    .get();

```