---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 493997bf6c5a85936fb5f81170620e0a37641e0529df61915131549b2f77ca4a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/publications/{id}')
    .version('beta')
    .delete();

```