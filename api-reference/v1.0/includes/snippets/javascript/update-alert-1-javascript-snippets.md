---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57c414b0d8c38f87432eb50be3280719a0309f84
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: 'String',
  closedDateTime: 'String (timestamp)',
  comments: [
    'String'
  ],
  feedback: '@odata.type: microsoft.graph.alertFeedback',
  status: '@odata.type: microsoft.graph.alertStatus',
  tags: [
    'String'
  ],
  vendorInformation: {
    provider: 'String',
    vendor: 'String'
  }
};

await client.api('/security/alerts/{alert_id}')
    .update(alert);

```