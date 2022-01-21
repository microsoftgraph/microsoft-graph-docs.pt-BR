---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c32f2c80c697ef1d21e8fa13b0762d8e18cd2bd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136275"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationCategory = {
  displayName: 'Quizzes'
};

await client.api('/education/classes/60eaa744-aa87-4276-b985-1633683119f8/assignmentCategories')
    .post(educationCategory);

```