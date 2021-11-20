---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e91050c89507bec126fad0ee5ac24936b52f4f29c2760051f6fd463def0f23d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let thumbnails = await client.api('/me/drive/items/{item-id}/thumbnails')
    .version('beta')
    .get();

```