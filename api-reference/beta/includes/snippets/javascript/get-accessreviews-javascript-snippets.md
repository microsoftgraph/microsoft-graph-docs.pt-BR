---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cf8a7be504ea554cefc7f424f7d908856de8014
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews')
    .version('beta')
    .filter('businessFlowTemplateId+eq+'6E4F3D20-C5C3-407F-9695-8460952BCC68'')
    .get();

```