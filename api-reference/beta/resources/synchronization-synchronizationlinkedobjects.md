---
title: Tipo de recurso synchronizationLinkedObjects
description: Representa todas as referências a serem provisionadas durante o provisionamento sob demanda.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 27053821607e8a813c690e18aa658256c0ff1038
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645582"
---
# <a name="synchronizationlinkedobjects-resource-type"></a>Tipo de recurso synchronizationLinkedObjects

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa todas as referências a serem provisionadas durante o provisionamento sob demanda.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|membros|[Coleção synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Todos os membros do grupo que você deseja provisionar.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationLinkedObjects"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationLinkedObjects",
  "members": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```
