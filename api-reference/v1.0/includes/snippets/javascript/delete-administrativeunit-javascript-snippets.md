---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 493f2ac4f5eb22fc261e192d0a04e38febe812da4e362c4efadf2e39297b2181
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/administrativeUnits/{id}')
    .delete();

```