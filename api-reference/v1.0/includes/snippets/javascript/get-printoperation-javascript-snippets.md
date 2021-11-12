---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32a6ce3ea179114656d2e95b1a18226a777767a54897155c5697dd3138a40d49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printOperation = await client.api('/print/operations/{printOperationId}')
    .get();

```