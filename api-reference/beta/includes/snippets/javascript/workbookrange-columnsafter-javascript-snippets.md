---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35aff41c8d3b1223ed8f5716714a9bd4e1570d8d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614697"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)')
    .version('beta')
    .post();

```