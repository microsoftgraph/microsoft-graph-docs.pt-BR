---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd4d4a8a230321c7e8e4d4db18c9c37d95c88feb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .post();

```