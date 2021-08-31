---
title: Tipo de recurso assignmentFilterValidationResult
description: Representa o resultado da API de validação.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9612d33c1e838eb5effaea555d8453b8acf6c1fe
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58807241"
---
# <a name="assignmentfiltervalidationresult-resource-type"></a>Tipo de recurso assignmentFilterValidationResult

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o resultado da API de validação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isValidRule|Boleano|Indicador para regra válida ou inválida.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterValidationResult",
  "isValidRule": true
}
```



