---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce772a8d1cdd1654de0175e8b330fafc35ac3abc
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "35723394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/rejectedSenders/$ref')
    .delete();

```