---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 544a3560d37a5277b5e0728a335e3d4015df1f16
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-title}')
    .version('beta')
    .get();

```