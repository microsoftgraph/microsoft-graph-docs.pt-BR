---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 413befacdbd50b84e20d90eaba0f84acd55df12ceec25f660c806251413e5c25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103058"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/deletedItems/{object-id}/restore')
    .post();

```