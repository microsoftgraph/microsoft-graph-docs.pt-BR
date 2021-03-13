---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63bc6e1cae39fbdab7854bcd44eb87289bf7468a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReview = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d')
    .version('beta')
    .get();

```