---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3de8f1623c6ed95ea139a2dd310f8cd8a4faa1caf0968f14aba16ef9a2a5b5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 4
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt')
    .post(workbookTableRow);

```