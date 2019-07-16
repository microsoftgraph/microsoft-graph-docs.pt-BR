---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2b644a0e6a963d061fcee8678faab16a0c318b2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736268"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains')
    .get();

```