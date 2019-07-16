---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5926ba2e6c6737a51846d78ec92984ba6736a139
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range')
    .get();

```