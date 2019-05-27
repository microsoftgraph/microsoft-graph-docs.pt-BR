---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3e639af0aee8cf1ce5fc456b52b29600e87d18c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions')
    .filter('id eq 'graphlearn_test'')
    .get();

```