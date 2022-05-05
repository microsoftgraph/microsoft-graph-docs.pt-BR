---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70df33d30b2da08f7b272eac01f416530d04182a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .select('ext55gb1l09_msLearnCourses')
    .get();

```