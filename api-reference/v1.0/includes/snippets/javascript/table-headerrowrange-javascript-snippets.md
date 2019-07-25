---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcc4965903ea27c02f59dc65688dab46a117ae17
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723051"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange')
    .post();

```