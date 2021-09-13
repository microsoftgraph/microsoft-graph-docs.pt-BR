---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b820d0ba8e318ac1140b2d3bf15848cc30900264d319fe0cb45e9412c0db701d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329898"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSchool = await client.api('/education/schools/{educationSchoolId}')
    .get();

```