---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee97128dda62ba471ea14e42aa7540be2eabf391e7c050e26cf8e299a04f3822
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327970"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let content = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content')
    .version('beta')
    .get();

```