---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb8c87166cd7729ad3ddd010ebad0a9189029207
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{class-id}/members/{member-id}')
    .delete();

```