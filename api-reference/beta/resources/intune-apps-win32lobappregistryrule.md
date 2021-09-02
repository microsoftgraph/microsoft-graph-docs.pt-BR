---
title: Tipo de recurso win32LobAppRegistryRule
description: Um tipo complexo para armazenar dados de regra do Registro para um aplicativo LOB win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7bf08b8a22ee8ce94de69bc57a9afb587b9bcfc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783985"
---
# <a name="win32lobappregistryrule-resource-type"></a>Tipo de recurso win32LobAppRegistryRule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar dados de regra do Registro para um aplicativo LOB win32.


Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|O tipo de regra que indica a finalidade da regra. Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Os valores possíveis são: `detection` e `requirement`.|
|check32BitOn64System|Boleano|Um valor que indica se o registro de 32 bits deve ser pesquisado em sistemas de 64 bits.|
|keyPath|Cadeia de caracteres|O caminho completo da entrada do Registro contendo o valor a ser detectado.|
|valueName|Cadeia de caracteres|O nome do valor do Registro a ser detectado.|
|operationType|[win32LobAppRegistryRuleOperationType](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|O tipo de operação do Registro. Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|O operador para detecção do Registro. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|Cadeia de caracteres|O valor de comparação do Registro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRule",
  "ruleType": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```



