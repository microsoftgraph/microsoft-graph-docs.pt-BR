---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe61eb58561be5c5efff6abe56e8ee48800e6df755c1efaf9339e7adb855228c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const abort = {
  reason: 'String'
};

await client.api('/print/printers/{printerId}/jobs/{printJobId}/abort')
    .post(abort);

```