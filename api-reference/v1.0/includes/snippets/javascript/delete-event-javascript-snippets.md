---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f155d22ffbb26993694d34b9d786e2251730a190
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}')
    .delete();

```