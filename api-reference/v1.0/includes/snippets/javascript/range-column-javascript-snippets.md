---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a92bd01e38dedce8f95e93459b18272152b9f064
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735990"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)')
    .get();

```