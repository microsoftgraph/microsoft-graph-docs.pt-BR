---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94e61edfb05f126321136c1477636b88a3ff01ef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508336"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}')
    .delete();

```