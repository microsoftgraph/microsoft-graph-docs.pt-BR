---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8507936454ad13a21c302b1f0700386b4a526eb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions')
    .get();

```