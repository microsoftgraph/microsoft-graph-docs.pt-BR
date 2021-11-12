---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 593f0e5c6b03ec592cd4e64094891421ff2107db62cbaaa279835b42ea743d03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChart = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .version('beta')
    .get();

```