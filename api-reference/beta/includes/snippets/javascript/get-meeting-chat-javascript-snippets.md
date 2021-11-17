---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3480a5a3e962aa365e3b90edcc593c14db8b82b6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/chats/19:meeting_ZDZlYTYxOWUtYzdlMi00ZmMxLWIxMTAtN2YzODZlZjAxYzI4@thread.v2')
    .version('beta')
    .get();

```