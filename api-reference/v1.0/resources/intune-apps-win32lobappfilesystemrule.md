---
title: Tipo de recurso win32LobAppFileSystemRule
description: Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a0c8a45a9f3d49c671949a2b5ad3b9bd549ee8d7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752396"
---
# <a name="win32lobappfilesystemrule-resource-type"></a>Tipo de recurso win32LobAppFileSystemRule

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB win32.


Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|O tipo de regra que indica a finalidade da regra. Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Os valores possíveis são: `detection` e `requirement`.|
|caminho|String|O arquivo ou o caminho da pasta a ser olhado para cima.|
|fileOrFolderName|Cadeia de caracteres|O arquivo ou o nome da pasta a ser olhado.|
|check32BitOn64System|Booliano|Um valor que indica se as variáveis de ambiente devem ser expandidas no contexto de 32 bits em sistemas de 64 bits.|
|operationType|[win32LobAppFileSystemOperationType](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|O tipo de operação do sistema de arquivos. Os possíveis valores são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|O operador para detecção de arquivo ou pasta. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|Cadeia de caracteres|O valor de comparação de arquivo ou pasta.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRule",
  "ruleType": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




