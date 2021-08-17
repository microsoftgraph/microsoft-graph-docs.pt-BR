---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b13383c7c59b24a2b89e90c335f7eaa44ede705e5e1cbfec57e7cf399c58eeaa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationRubric = await client.api('/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d')
    .get();

```