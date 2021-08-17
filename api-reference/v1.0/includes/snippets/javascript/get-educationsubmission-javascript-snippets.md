---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2ca48a1654a042832dede929744b206c4ab18ca79529cbd77f0b7a8fd24582b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330049"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSubmission = await client.api('/education/classes/11010/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/33223')
    .get();

```