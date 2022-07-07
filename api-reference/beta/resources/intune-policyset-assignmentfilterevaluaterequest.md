---
title: Tipo de recurso assignmentFilterEvaluateRequest
description: Solicitação de avaliação de filtro de atribuição para dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4a3dde68384dcf9813167544a8d2b56c8db7a98e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666855"
---
# <a name="assignmentfilterevaluaterequest-resource-type"></a>Tipo de recurso assignmentFilterEvaluateRequest

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Solicitação de avaliação de filtro de atribuição para dispositivos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|plataforma|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Tipo de plataforma dos dispositivos nos quais o Filtro de Atribuição será aplicável. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|Regra|Cadeia de caracteres|Definição de regra do Filtro de Atribuição.|
|top|Int32|Limite de registros por solicitação. O valor padrão é 100, se fornecido menor que 0 ou maior que 100|
|skip|Int32|Número de registros a serem ignorados. O valor padrão é 0|
|Orderby|Coleção de cadeias de caracteres|Ordem em que os dispositivos devem ser classificados. O padrão é crescente no nome do dispositivo.|
|search|Cadeia de caracteres|Palavra-chave de pesquisa aplicada aos dispositivos encontrados no escopo.|

## <a name="relationships"></a>Relações
Nenhum

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
  ],
  "search": "String"
}
```




