---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2be1e1c9d6e1d2a7d80192553f80820743250f63
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails?select=c300x400_Crop')
    .get();

```