---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b600d8b77e355ef8802d623529ab68723de0fb9a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let historyDefinitions = await client.api('/identityGovernance/accessReviews/historyDefinitions')
    .get();

```