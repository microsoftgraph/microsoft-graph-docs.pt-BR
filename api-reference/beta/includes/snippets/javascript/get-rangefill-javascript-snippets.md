---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5de1f765029cce30aa084d6acaa8983320d1da32f06cb3b63d1015e1bb6fec8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFill = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .version('beta')
    .get();

```