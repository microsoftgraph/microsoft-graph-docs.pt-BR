---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd2fe5c4374fb24d1e5209b1b7a6fe1ad55080fb499188cf5ad4fd4880c98c6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .version('beta')
    .post();

```