---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82fc93d87fdf03af7bf0bd687fb0cb483c05cabd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .get();

```