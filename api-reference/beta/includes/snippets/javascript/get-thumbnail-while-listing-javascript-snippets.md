---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 200710c51631c556794ee312311f17b559c93c150ff29bd5fa288b600be6a3b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327971"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/items/{item-id}/children')
    .version('beta')
    .expand('thumbnails')
    .get();

```