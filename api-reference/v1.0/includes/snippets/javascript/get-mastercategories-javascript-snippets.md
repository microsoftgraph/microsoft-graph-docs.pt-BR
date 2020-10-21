---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b726144e389f2c994f1f278ffc9d0931c21972ab
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories')
    .get();

```