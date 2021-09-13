---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1dbbc5b4d0d7aba15e7a38ddc717d4668250e976d0b2c5b0a2ce8e54376ccfc5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214794"
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