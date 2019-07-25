---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f35aa75d9c36b0d8d119ec0d4a3cd289e91e0967
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .version('beta')
    .update({workbookRangeFill : workbookRangeFill});

```