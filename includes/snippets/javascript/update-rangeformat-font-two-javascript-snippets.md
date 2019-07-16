---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e300ce3bd1cde8c8a7daf27dc31747f380ec9c1f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  italic: true,
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font')
    .update({workbookRangeFont : workbookRangeFont});

```