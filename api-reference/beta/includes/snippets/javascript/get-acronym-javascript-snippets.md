---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 836183f033567f27d823b75138f0fd9252154f3e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338164"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let acronym = await client.api('/search/acronyms/{acronymsId}')
    .version('beta')
    .get();

```