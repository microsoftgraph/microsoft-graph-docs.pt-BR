---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d030ccd92fbd27f23cae5e52b4730233f4735a3d0fb7876358b1cdc72a0b243
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .version('beta')
    .get();

```