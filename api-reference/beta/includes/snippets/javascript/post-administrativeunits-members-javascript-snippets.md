---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57a32106b83572c7eade78f8597180bd405dd503
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/beta/groups/{id}'
};

await client.api('/administrativeUnits/{id}/members/$ref')
    .version('beta')
    .post(directoryObject);

```