---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a427497fa6c99425c7fd27be15cd48fda158a9e7
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/policies/{id}')
    .delete();

```