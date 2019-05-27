---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60deca817222e9b7b680f8210a462ecdb31c7709
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
      displayName:"Project expenses",
      color:"preset9"
};

let res = await client.api('/me/outlook/masterCategories')
    .post({outlookCategory : outlookCategory});

```