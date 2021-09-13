---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac10508fc7ba9854fd95b2f02c5567fc9406d418b2bfb9bf46b4894171040c9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/appCatalogs/teamsApps?requiresReview=true')
    .post();

```