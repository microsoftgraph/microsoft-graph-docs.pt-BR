---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87bb63d7d5c22405bc45b99e247388d0ec4df904d7e1b24ea9fb93d6fbad653b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let thumbnails = await client.api('/me/drive/items/{item-id}/thumbnails?select=c300x400_crop')
    .get();

```