---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e9244f62bf7857aa08c8b53a68bb8d736ef588a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499239"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails')
    .version('beta')
    .get();

```