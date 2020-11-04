---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba1027e4a44691809521291ef9858ae32a2228a2
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists/AAMkADIyAAAhrbPXAAA=')
    .delete();

```