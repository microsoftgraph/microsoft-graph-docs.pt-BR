---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d454c47825910066996d4c687c931ba3bb9f5b609afc9eb4ac0d194666a06183
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartAxisTitle = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title')
    .get();

```