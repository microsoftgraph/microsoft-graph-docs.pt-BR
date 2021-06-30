---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6fdf0c822687f9f8e1d56758021b48bda1a9659f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207178"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let int32 = await client.api('/groups/{id}/transitiveMembers/$count')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .get();

```