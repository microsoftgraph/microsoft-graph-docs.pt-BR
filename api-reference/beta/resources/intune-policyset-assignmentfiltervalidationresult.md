---
title: Tipo de recurso assignmentFilterValidationResult
description: Representa o resultado da API de validação.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 69006f9582b5f9a1c2172b3d2fa2f43b07998985
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074910"
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



