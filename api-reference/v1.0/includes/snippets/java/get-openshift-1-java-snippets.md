---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4cee749365d80f406a76270ee86670c1b8046f7e9a3f006fd37cc0f46dbaea74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214355"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenShift openShift = graphClient.teams("{id}").schedule().openShifts("OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8")
    .buildRequest()
    .get();

```