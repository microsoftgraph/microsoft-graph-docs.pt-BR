---
title: Tipo de recurso win32LobAppFileSystemRequirement
description: Contém arquivo ou caminho de pasta para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa212f952f9b4fa87e5916dfbc02de694b6cb030
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790182"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a>Tipo de recurso win32LobAppFileSystemRequirement

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém arquivo ou caminho de pasta para detectar um aplicativo Win32


Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|O operador para detecção Herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md). Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detectionValue|Cadeia de caracteres|O valor de detecção Herdado [de win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|caminho|String|O arquivo ou o caminho da pasta para detectar o aplicativo Win32 Line of Business (LoB)|
|fileOrFolderName|Cadeia de caracteres|O arquivo ou o nome da pasta para detectar o aplicativo Win32 Line of Business (LoB)|
|check32BitOn64System|Boleano|Um valor que indica se esse arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits|
|detectionType|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|O tipo de detecção do sistema de arquivos. Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRequirement",
  "operator": "String",
  "detectionValue": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String"
}
```



