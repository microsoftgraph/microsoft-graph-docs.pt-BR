---
title: Tipo de recurso deviceManagementSettingComparison
description: Entidade que representa o resultado da comparação de configuração
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a2f9dca86529821f24840e209ef10c25014d27b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091402"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>Tipo de recurso deviceManagementSettingComparison

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o resultado da comparação de configuração

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID de configuração|
|displayName|Cadeia de caracteres|O nome de exibição da configuração|
|definitionId|Cadeia de Caracteres|A ID da definição de configuração para esta instância|
|currentValueJson|Cadeia de Caracteres|Representação JSON do valor da configuração do modelo de intenção atual (ou)|
|newValueJson|Cadeia de Caracteres|Representação JSON do valor da configuração do novo modelo|
|comparisonResult|[deviceManagementComparisonResult](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|Definindo o resultado da comparação. Os valores possíveis são: `unknown`, `equal`, `notEqual`, `added`, `removed`.|

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



