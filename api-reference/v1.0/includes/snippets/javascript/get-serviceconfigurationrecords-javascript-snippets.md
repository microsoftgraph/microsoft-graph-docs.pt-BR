---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30d354ee47e4bc4cfcc9ef85d0a9837b16037e32
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465865"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/{domain-name}/serviceConfigurationRecords')
    .get();

```