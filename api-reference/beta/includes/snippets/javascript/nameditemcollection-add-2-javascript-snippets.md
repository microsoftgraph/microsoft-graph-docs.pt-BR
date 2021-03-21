---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6009200e302751ff81d7e65e31d869184debc76
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  name: 'test7',
  formula: '=SUM(Sheet2!$A$1+Sheet2!$A$2)',
  comment: 'Comment for the named item'
};

await client.api('/me/drive/items/{id}/workbook/names/addFormulaLocal')
    .version('beta')
    .post(workbookNamedItem);

```