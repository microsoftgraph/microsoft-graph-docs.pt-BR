---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4a555873247d777926bf0a85b18ed8af0ec554c381487ae4c4b154c812ca74a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const restart = {
   criteria: {
       resetScope: 'Watermark, Escrows, QuarantineState'
   }
};

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart')
    .version('beta')
    .post(restart);

```