---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1362515270e16ae22b334794ca4a630f263951b2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subjectRightsRequests = await client.api('/privacy/subjectRightsRequests')
    .get();

```