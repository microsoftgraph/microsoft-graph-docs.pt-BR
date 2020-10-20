---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96f3b866ba9f8195b8a16ac06cbf3a6f747e39ba
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620474"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const merge = {
  across: true
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/merge')
    .version('beta')
    .post(merge);

```