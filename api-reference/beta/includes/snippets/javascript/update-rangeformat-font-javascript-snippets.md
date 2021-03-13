---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92176e089f87ff077377446643cceb1811159a8d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: '#4B180E',
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font')
    .version('beta')
    .update(workbookRangeFont);

```