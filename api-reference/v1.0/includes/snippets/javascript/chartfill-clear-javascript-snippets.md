---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 933b345af1797900ae9609283296dfb3f29cd56548916e740421fe9fd27ad5a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear')
    .post();

```