---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7640294f75e067f529f561dca0084ba9259bb6b27f9f35158d008b474bab1156
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}')
    .version('beta')
    .delete();

```