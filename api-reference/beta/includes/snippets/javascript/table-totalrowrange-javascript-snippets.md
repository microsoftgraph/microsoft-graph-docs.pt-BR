---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 097a43f31f90a685ea558bac8e173e4979e55bfe1c6214dde25b5100e97a3c46
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100362"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/TotalRowRange')
    .version('beta')
    .get();

```