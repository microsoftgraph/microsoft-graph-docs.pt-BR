---
title: Tipo de recurso win32LobAppFileSystemRule
description: Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB win32.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d95da930022085f157be0141e9d8a3cd54b35a31
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127539"
---
# <a name="win32lobappfilesystemrule-resource-type"></a>Tipo de recurso win32LobAppFileSystemRule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB win32.


Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|O tipo de regra que indica a finalidade da regra. Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Os valores possíveis são: `detection` e `requirement`.|
|caminho|String|O arquivo ou o caminho da pasta a ser olhado para cima.|
|fileOrFolderName|Cadeia de Caracteres|O arquivo ou o nome da pasta a ser olhado.|
|check32BitOn64System|Boleano|Um valor que indica se as variáveis de ambiente devem ser expandidas no contexto de 32 bits em sistemas de 64 bits.|
|operationType|[win32LobAppFileSystemOperationType](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|O tipo de operação do sistema de arquivos. Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|O operador para detecção de arquivo ou pasta. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|Cadeia de Caracteres|O valor de comparação de arquivo ou pasta.|

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



