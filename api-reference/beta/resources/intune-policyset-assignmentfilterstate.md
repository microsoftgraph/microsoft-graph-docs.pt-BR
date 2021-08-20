---
title: Tipo de recurso assignmentFilterState
description: Representa o resultado da API GetState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3f980acee0915e5bae7eb3f4dd1c910e9c3f7fb09f126091667c9235ecab9719
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133093"
---
# <a name="assignmentfilterstate-resource-type"></a>Tipo de recurso assignmentFilterState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o resultado da API GetState.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enabled|Boolean|Indicador para se AssignmentFilter estiver habilitado ou desabilitado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterState",
  "enabled": true
}
```




