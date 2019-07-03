---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13adc7c6b052a947a956baf4eefcc9eb92d96dc3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: 3
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt')
    .post({workbookTableColumn : workbookTableColumn});

```