---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2991136928e5293f85971456335df56f47cccd11e2c7f687da14b0a72ec6954d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let content = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content')
    .get();

```