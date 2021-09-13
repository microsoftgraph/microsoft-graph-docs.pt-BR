---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0ace877a7e4bd64c53e664f094e3276938775373291fe96b4f6eac6aa5ea703
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnits = await client.api('/directory/administrativeUnits')
    .get();

```