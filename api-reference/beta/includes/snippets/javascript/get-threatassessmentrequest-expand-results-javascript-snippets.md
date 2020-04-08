---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76aeef4b760d28c7e4b31eb04e51eed31e6bd06f
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "40867132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996')
    .version('beta')
    .expand('results')
    .get();

```