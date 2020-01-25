---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a4196941ac36da346d1f172d661ed4a65299c70
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41494520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{id}/workbook/comments/{id}/replies/{id}')
    .get();

```