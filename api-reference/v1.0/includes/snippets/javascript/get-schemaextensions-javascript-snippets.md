---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3e639af0aee8cf1ce5fc456b52b29600e87d18c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615647"
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