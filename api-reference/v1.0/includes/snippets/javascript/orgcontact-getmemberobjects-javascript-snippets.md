---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b42a7fee9ea2bc74d6c2936ae28316b8a9c9bda9
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

let res = await client.api('/contacts/{id}/getMemberObjects')
    .post(string);

```