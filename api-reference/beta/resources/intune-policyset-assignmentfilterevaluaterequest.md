---
title: Tipo de recurso assignmentFilterEvaluateRequest
description: Solicitação de avaliação de filtro de atribuição para dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee45c31df0eb2bdd8f65eb670af4a3a83b64f0b9
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63368158"
---
# <a name="assignmentfilterevaluaterequest-resource-type"></a>Tipo de recurso assignmentFilterEvaluateRequest

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Solicitação de avaliação de filtro de atribuição para dispositivos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|plataforma|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Tipo de plataforma dos dispositivos nos quais o Filtro de Atribuição será aplicável. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|rule|String|Definição de regra do Filtro de Atribuição.|
|top|Int32|Limite de registros por solicitação. O valor padrão é 100, se fornecido menor que 0 ou maior que 100|
|skip|Int32|Número de registros a ignorar. O valor padrão é 0|
|orderBy|String collection|Ordem em que os dispositivos devem ser organizados. O padrão é crescente no nome do dispositivo.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluateRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluateRequest",
  "platform": "String",
  "rule": "String",
  "top": 1024,
  "skip": 1024,
  "orderBy": [
    "String"
  ]
}
```




