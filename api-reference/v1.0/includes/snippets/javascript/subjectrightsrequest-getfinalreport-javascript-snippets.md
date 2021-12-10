---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4bf5c0ad91fe8bc030e54ccaf2861fe7245d6cf
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687572"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalReport')
    .get();

```