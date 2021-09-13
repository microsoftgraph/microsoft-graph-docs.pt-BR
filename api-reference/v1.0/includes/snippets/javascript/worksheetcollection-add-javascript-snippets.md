---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8723eadacfcd43f87dfc1980834d6dd7b057b54fa2ccd873a9a75e9989a9196
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329825"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookWorksheet = {
  name: 'name-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/add')
    .post(workbookWorksheet);

```