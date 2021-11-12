---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6ad11c465d2dfdad42b4e13da5e64450cfb1f3029e8f4414346638f74251e6ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101443"
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