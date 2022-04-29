---
title: Tipo complexo subjectSet
description: O tipo base abstrato para tipos usados nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0a266aea0693c6faf994da0fd829b8cacdee619e
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133115"
---
# <a name="subjectset-complex-type"></a>Tipo complexo subjectSet

Namespace: microsoft.graph

Um objeto compartilhado que é usado em políticas de atribuição de pacote de acesso de gerenciamento de direitos e políticas de gerenciamento de função.

+ No gerenciamento de direitos, usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote de acesso.
+ Nas políticas de gerenciamento de funções, usadas nas configurações de aprovação definidas em regras para políticas de gerenciamento de função.

Esse é um tipo base abstrato herdado pelos seguintes tipos derivados:
+ [singleUser](singleuser.md)
+ [singleServicePrincipal](singleserviceprincipal.md)
+ [groupMembers](groupmembers.md)
+ [connectedOrganizationMembers](connectedorganizationmembers.md)
+ [requestorManager](requestormanager.md)
+ [internalSponsors](internalsponsors.md)
+ [externalSponsors](externalsponsors.md)
+ [targetManager](targetmanager.md)
+ [targetApplicationOwners](targetapplicationowners.md)


## <a name="properties"></a>Propriedades

Nenhum.
## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectSet"
}
```


