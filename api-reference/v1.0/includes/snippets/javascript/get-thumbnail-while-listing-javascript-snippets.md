---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1ed88ab6b39540c3a147ff5c3f83410949c6d23a11f9b1b21f32b73d2b36a12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/items/{item-id}/children')
    .expand('thumbnails')
    .get();

```