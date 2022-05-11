---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45f2c04d63ba9a5dc528d33c9bac1d7b85d02bae
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getCompatibleHubContentTypes = await client.api('/sites/root/lists/Documents/contentTypes/getCompatibleHubContentTypes')
    .get();

```