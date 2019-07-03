---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd369fb3dca0090a68fab8a8eb5ca0dccb7cb818
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScoreControlProfiles')
    .get();

```