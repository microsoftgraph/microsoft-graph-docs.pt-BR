---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 943515909a51623043590f201f4dd7d8e70bd35d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const apply = {
  criteria: {
    criterion1: "criterion1-value",
    criterion2: "criterion2-value",
    color: "color-value",
    operator: {
    },
    icon: {
      set: "set-value",
      index: 99
    },
    dynamicCriteria: "dynamicCriteria-value",
    values: {
    },
    filterOn: "filterOn-value"
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply')
    .version('beta')
    .post(apply);

```