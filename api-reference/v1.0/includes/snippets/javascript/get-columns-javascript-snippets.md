---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3be52b0bb1ec202d5f792561414c2577818bf867d0e984f463ff77bdfa6bcb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .skip(5)
    .top(5)
    .get();

```