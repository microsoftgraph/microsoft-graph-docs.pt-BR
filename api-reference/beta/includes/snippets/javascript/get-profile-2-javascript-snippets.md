---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2da69a74e708c1a05d37993544bfb5213a0ade22
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profile = await client.api('/me/profile')
    .version('beta')
    .expand('skills($select=displayName)')
    .get();

```