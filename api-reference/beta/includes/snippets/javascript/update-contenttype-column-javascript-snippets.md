---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2531ac990f4692ad0d5e66ec528e862b1974ec150e0c25d1d071cda98c401ae9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const columnDefinition = {
  required: true,
  hidden: false,
  propagateChanges: false       
};

await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}')
    .version('beta')
    .update(columnDefinition);

```