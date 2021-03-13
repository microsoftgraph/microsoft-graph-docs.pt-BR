---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f32bcccae079aef7baaed881de5907e444afdc60
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)')
    .version('beta')
    .get();

```