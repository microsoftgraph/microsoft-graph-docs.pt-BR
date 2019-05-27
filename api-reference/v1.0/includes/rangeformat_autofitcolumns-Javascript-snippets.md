---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26857d170c5a4c45ec0fcb13e990d5f7c739e421
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns')
    .post();

```