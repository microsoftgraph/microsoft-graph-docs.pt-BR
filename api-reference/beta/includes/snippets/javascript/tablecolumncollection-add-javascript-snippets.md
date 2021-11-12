---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 070de53b473c9aa84374effe89d5107ebd845e775eadbfc655d77e240edd7ad5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: {
  },
  values: [
    {
    }
  ]
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/add')
    .version('beta')
    .post(workbookTableColumn);

```