---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69b028086b11011ed69c84370389424483cf557f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)')
    .get();

```