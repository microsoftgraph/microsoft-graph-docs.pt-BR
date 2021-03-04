---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 206ef33e32cac3eca1dbf1a40800c376b988282a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/TotalRowRange')
    .version('beta')
    .get();

```