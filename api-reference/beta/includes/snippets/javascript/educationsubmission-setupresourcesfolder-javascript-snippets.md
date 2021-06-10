---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c24b9cd117869a63c0524d22bbca87f12670f96
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870126"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSubmission = {
};

await client.api('/education/classes/11012/assignments/19002/submissions/20302/setUpResourcesFolder')
    .version('beta')
    .post(educationSubmission);

```