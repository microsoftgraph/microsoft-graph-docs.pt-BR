---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09c2bd012eb5a66efc907bf9eb9f16710fa021490f358d77606211bd9715aa57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100225"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeSort = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/sort')
    .get();

```