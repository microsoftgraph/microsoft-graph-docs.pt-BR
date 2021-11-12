---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a97c4a0a94097c6caf94ace193a6d5d40cb2b4960264392e96f732f69683aab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159935"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().plans("xqQg5FS2LkCp935s-FIFm2QAFkHM").tasks()
    .buildRequest()
    .get();

```