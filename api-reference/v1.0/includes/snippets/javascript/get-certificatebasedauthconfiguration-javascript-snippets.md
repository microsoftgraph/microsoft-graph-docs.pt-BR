---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05f246a56590a46007ea5d7219c2aecb530b9332
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .get();

```