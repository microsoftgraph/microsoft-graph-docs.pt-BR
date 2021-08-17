---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6895be6b1e7cb35aad7a1bfbc7b2b08efe93eb9938ec05844767ea203a8fd4c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .header('ConsistencyLevel','eventual')
    .search('displayName:wa')
    .get();

```