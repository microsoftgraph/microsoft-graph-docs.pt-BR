---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a7f3ce942c89e3d66727ae777e097bca79f7f31a73b40660f44b5ce65f5ba77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271896"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/LastCell')
    .version('beta')
    .get();

```