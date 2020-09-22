---
title: tipo de recurso deviceManagementSettingComparison
description: Entidade que representa o resultado da comparação da configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e51d413dfa0e1e60fcf07e37c2806c39f62cc76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061242"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>tipo de recurso deviceManagementSettingComparison

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o resultado da comparação da configuração

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da configuração|
|displayName|Cadeia de caracteres|O nome de exibição da configuração|
|DefinitionId|Cadeia de caracteres|A ID da definição de configuração dessa instância|
|currentValueJson|Cadeia de caracteres|Representação JSON do valor da configuração de modelo de intenção atual (ou)|
|newValueJson|Cadeia de caracteres|Representação JSON do valor da configuração de um novo modelo|
|comparisonResult|[deviceManagementComparisonResult](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|Configurando o resultado da comparação. Os valores possíveis são: `unknown`, `equal`, `notEqual`, `added`, `removed`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```






