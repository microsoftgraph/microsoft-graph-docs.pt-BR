---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 899e12dd3337624b13af6410e2bf806516aa0330
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/v1.0/education/users/14011'
};

await client.api('/education/classes/{class-id}/teachers/$ref')
    .post(educationUser);

```