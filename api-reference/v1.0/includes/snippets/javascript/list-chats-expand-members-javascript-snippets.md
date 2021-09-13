---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd6c311e9388a9de5d925e545cdd3a35f4e8a654
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chats = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats')
    .expand('members')
    .get();

```