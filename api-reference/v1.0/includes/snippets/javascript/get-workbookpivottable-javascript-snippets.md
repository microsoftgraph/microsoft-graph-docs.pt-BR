---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1fe431641853e4e69d70077eecc254e0d85f6f1f59e406e77248270c7e69230c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookPivotTable = await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}')
    .get();

```