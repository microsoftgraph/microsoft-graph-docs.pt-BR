---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2b644a0e6a963d061fcee8678faab16a0c318b2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492127"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains')
    .get();

```