---
title: tipo de recurso win32LobAppFileSystemRule
description: Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e45db436201b339f075f35d3865c8d0c84f1ea6d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274030"
---
# <a name="win32lobappfilesystemrule-resource-type"></a>tipo de recurso win32LobAppFileSystemRule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB Win32.


Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|O tipo de regra que indica o objetivo da regra. Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Os valores possíveis são: `detection` e `requirement`.|
|caminho|String|O caminho do arquivo ou da pasta a ser pesquisado.|
|fileOrFolderName|String|O nome do arquivo ou pasta a ser procurado.|
|check32BitOn64System|Booliano|Um valor que indica se as variáveis de ambiente serão expandidas no contexto de 32 bits em sistemas de 64 bits.|
|OperationType|[win32LobAppFileSystemOperationType](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|O tipo de operação do sistema de arquivos. Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|O operador para detecção de arquivo ou pasta. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|ComparisonValue|String|O valor de comparação de arquivo ou pasta.|

## <a name="relationships"></a>Relações
Nenhum

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




