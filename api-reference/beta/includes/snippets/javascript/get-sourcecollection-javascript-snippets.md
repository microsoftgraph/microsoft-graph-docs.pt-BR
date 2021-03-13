---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5369dde9eeaba8fc84d305b9ebd23ecef4643ab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sourceCollection = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119')
    .version('beta')
    .expand('lastEstimateStatisticsOperation')
    .get();

```