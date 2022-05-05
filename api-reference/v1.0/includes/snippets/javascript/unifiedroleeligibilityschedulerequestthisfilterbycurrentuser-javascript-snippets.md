---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9adc05d6e1be357f73495de73a7643d66e375645
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/roleEligibilityScheduleRequests/filterByCurrentUser(on='principal')')
    .get();

```