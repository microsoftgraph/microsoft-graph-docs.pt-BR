---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea9135994485057d1147620411f6f5552b2b4b13
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover')
    .version('beta')
    .post();

```