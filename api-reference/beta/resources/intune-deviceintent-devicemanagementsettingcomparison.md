---
title: tipo de recurso deviceManagementSettingComparison
description: Entidade que representa o resultado da comparação da configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e8c886e3464070d0dba8779741ed65681a764de
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364737"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>tipo de recurso deviceManagementSettingComparison

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o resultado da comparação da configuração

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da configuração|
|displayName|String|O nome de exibição da configuração|
|DefinitionId|String|A ID da definição de configuração dessa instância|
|currentValueJson|String|Representação JSON do valor da configuração de modelo de intenção atual (ou)|
|newValueJson|String|Representação JSON do valor da configuração de um novo modelo|
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



