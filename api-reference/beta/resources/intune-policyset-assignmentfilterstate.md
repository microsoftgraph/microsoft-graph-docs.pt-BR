---
title: Tipo de recurso assignmentFilterState
description: Representa o resultado da API GetState.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 83837ee64983e657e37c6a4de44b79a3fe87bd0f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074987"
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



