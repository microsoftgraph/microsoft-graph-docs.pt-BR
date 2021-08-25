---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98323016d2dd88113b9389ebfc802bbbac3270ba546dd15ef8632a1cc0325f2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273459"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversations = await client.api('/groups/{id}/conversations')
    .get();

```