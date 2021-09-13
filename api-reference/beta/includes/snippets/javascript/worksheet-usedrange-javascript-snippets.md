---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77743060f59aa0490a134e24a81e89f47118320a4913fe7704584d5f3250db5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)')
    .version('beta')
    .get();

```