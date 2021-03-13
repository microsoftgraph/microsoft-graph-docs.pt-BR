---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 786336e74df3239b69cd0003017c7cf39556f74c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: 'focused',
  senderEmailAddress: {
    name: 'Samantha Booth',
    address: 'samanthab@adatum.onmicrosoft.com'
  }
};

await client.api('/me/inferenceClassification/overrides')
    .version('beta')
    .post(inferenceClassificationOverride);

```