---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e156821dd9684bc82921b3e82c3fe39586b1e8dd5225efdc4a7f1ff57ee4f249
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onenoteSection = await client.api('/me/onenote/sections/{id}')
    .version('beta')
    .get();

```