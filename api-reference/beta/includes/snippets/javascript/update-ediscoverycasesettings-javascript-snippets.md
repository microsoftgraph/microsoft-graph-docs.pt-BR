---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5bfe038fdd85fb17a92024a68e661fb63f86c680
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryCaseSettings = {
  '@odata.type': '#microsoft.graph.security.ediscoveryCaseSettings',
  redundancyDetection: {
    '@odata.type': 'microsoft.graph.security.redundancyDetectionSettings'
  },
  topicModeling: {
    '@odata.type': 'microsoft.graph.security.topicModelingSettings'
  },
  ocr: {
    '@odata.type': 'microsoft.graph.security.ocrSettings'
  }
};

await client.api('/security/cases/ediscoveryCases/{ediscoveryCaseId}/settings')
    .version('beta')
    .update(ediscoveryCaseSettings);

```