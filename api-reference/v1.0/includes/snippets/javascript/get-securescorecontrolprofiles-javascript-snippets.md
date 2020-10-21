---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd369fb3dca0090a68fab8a8eb5ca0dccb7cb818
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScoreControlProfiles')
    .get();

```