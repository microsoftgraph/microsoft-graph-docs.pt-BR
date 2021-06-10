---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 701c9dd745db81b2b36e496e6ab3c1dd4c336a00
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870371"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect')
    .post();

```