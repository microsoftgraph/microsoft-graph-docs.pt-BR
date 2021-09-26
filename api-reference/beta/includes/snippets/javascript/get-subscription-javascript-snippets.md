---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f73fef7bffdd42f387d60456f96498569fde6fc95fa7770e930c1aa169d78865
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156417"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscription = await client.api('/subscriptions/{id}')
    .version('beta')
    .get();

```