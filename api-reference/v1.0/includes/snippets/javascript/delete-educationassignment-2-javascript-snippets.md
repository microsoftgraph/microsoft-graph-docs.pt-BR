---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c89b52431347c287cfa0493b178cf240ef040ad6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignmentCategories/b93d3b6b-360c-45c0-8764-e8bb622a9504')
    .delete();

```