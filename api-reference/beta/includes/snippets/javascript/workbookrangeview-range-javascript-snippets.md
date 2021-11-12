---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9738ec1513706f242fac95abf1c10063609ed1a787e96abaaa281852efd8ee91
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range')
    .version('beta')
    .get();

```