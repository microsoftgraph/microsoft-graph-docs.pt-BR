---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0df75f7191666f597fe00ab546b3cac91cb812d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeView = await client.api('/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView')
    .version('beta')
    .get();

```