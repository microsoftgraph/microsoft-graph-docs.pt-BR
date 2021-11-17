---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0eaa6e6c19e961d57ff04594b95c8f2f970f0c03aa3bc29c2002af0834dc209b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: 'focused'
};

await client.api('/me/inferenceClassification/overrides/{id}')
    .version('beta')
    .update(inferenceClassificationOverride);

```