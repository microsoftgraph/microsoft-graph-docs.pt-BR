---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eafe77254e3d98807b6d6449c41b4371df7c625d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettings/{id}')
    .delete();

```