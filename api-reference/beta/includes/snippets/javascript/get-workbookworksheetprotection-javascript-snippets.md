---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31c567938c6549bdd49c7120c960c27c8dde27785bca659596f031339021e754
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookWorksheetProtection = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection')
    .version('beta')
    .get();

```