---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 809f5d481dc8a36fb22057c36ac72115cd375f96
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSchool = await client.api('/education/schools/{educationSchoolId}')
    .get();

```