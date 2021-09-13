---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4424732803e2a6c26bbfca91098c3ebf7a74f059406c77ec4c98c0ca5dba96d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215501"
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
    .post(workbookNamedItem);

```