---
title: Tipo de recurso deviceManagementSettingComparison
description: Entidade que representa o resultado da comparação de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28ca971dbfa41c9237ed9f6ff33579d5e9f4eeb5f2b32dbf0ffd3b0eca191424
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156202"
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
|definitionId|Cadeia de caracteres|A ID da definição de configuração para esta instância|
|currentValueJson|Cadeia de caracteres|Representação JSON do valor da configuração do modelo de intenção atual (ou)|
|newValueJson|Cadeia de caracteres|Representação JSON do valor da configuração do novo modelo|
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




