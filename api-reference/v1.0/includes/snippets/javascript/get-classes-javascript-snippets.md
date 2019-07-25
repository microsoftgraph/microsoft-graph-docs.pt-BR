---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd4bd4b547d96252742096699dde71251e50cddc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/classes')
    .get();

```