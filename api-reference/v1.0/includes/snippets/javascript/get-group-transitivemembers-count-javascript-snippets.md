---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 757f466cfa87aecc6ec54dbdd6e72d8465a66519dc704c6f44ade8b929718aca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326912"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let int32 = await client.api('/groups/{id}/transitiveMembers/$count')
    .header('ConsistencyLevel','eventual')
    .get();

```