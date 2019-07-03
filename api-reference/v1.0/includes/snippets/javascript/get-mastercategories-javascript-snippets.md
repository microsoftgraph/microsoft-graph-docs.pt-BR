---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b726144e389f2c994f1f278ffc9d0931c21972ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories')
    .get();

```