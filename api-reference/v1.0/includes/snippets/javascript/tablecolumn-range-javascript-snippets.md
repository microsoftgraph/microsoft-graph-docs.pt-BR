---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0762e10685c7c0e654a5ca67ace3603d22e9f7a4fd114b0acbb95f4e2f8dd21a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range')
    .get();

```