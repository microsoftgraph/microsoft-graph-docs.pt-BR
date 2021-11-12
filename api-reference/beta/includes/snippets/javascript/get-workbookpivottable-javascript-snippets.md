---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f40dfb6840064371f074040b87d9d4b5e3cebd88262650c4d6eb95d6584e4ef8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookPivotTable = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables/{id}')
    .version('beta')
    .get();

```