---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5499723ca095319f81136f8f7659e43cde2bea17
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41496054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{id}/workbook/comments/{id}')
    .version('beta')
    .get();

```