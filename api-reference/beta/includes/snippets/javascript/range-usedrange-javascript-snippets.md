---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59dc5129d63a4f83a18008b07b853e3cfdbdcdcdf7ef4c9319400e1a62af3228
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273526"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/UsedRange')
    .version('beta')
    .get();

```