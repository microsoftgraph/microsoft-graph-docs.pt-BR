---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6131bd1f22bc729d7ea91c06310b13acb63912c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442897"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/EntireRow')
    .version('beta')
    .get();

```