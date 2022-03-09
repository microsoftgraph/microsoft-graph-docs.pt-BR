---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84ed249e4f36205f388a583ab5dc10da2d2baa0f8e78197d6530cea06462b551
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/10001/classes/11001')
    .version('beta')
    .delete();

```