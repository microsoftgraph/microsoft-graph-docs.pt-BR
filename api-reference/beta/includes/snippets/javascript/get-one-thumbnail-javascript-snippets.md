---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b730335c53e54f0745cea78fb89c319df5df2fab434c90468faf877db1e26de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let response = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}')
    .version('beta')
    .get();

```