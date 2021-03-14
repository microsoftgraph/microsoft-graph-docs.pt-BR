---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd93edbb73c447795097fd51a88992ec0a519ca1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const convertIdResult = {
  inputIds: [
    '{rest-formatted-id-1}',
    '{rest-formatted-id-2}'
  ],
  sourceIdType: 'restId',
  targetIdType: 'restImmutableEntryId'
};

await client.api('/me/translateExchangeIds')
    .post(convertIdResult);

```