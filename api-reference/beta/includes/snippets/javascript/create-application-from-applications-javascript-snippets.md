---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 211271a40929c6655e1e1e2b1ce41c788d9b8896
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  allowPublicClient: true,
  displayName: "Display name"
};

let res = await client.api('/applications')
    .version('beta')
    .post(application);

```