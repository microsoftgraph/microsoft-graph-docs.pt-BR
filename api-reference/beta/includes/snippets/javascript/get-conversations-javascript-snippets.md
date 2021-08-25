---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f7b263509562e452762d7915710bebf9ac21b644442f2344f36cfda7e8f2f67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversations = await client.api('/groups/{id}/conversations')
    .version('beta')
    .get();

```