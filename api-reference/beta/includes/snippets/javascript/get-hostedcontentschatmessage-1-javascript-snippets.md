---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f209f502664d17ec301642f8b3648c6d72323108
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610358"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let hostedContents = await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents')
    .version('beta')
    .get();

```