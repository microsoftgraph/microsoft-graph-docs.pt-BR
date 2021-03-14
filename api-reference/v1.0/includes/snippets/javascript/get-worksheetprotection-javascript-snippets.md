---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3423546cf996975662b8afd2b87f4b5bc2b61ec4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookWorksheetProtection = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection')
    .get();

```