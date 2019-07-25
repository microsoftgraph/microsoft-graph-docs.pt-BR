---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60deca817222e9b7b680f8210a462ecdb31c7709
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732932"
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