---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64bd25085d81ab93622c5892f0ac199bd8353a60abbd843bee2041d74683f618
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChart = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .get();

```