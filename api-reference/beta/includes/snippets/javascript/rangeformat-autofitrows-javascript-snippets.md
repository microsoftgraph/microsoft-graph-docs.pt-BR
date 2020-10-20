---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d29edbb02d510c1c8440f4337cc3813c59eca3cd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows')
    .version('beta')
    .post();

```