---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecfdae3b766f9b2302c25a73cac0080b66810caea2bb81f68af5f38a7c4e0ee7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequest = await client.api('/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa')
    .version('beta')
    .get();

```