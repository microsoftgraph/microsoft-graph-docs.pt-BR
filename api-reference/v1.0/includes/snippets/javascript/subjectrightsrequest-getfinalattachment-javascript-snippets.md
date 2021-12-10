---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90abf67495402ea4700b1ead7ad9becb3163f98b
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687607"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment')
    .get();

```