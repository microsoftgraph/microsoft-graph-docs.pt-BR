---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9ccbee0f9739f039b9c156cbbdd74efdf787891b5f6fc90a6073f3341c0d4bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTable = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .version('beta')
    .get();

```