---
title: tipo de recurso de win32LobAppFileSystemDetection
description: Contém o caminho de arquivo ou pasta para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13a994d39ec42ddcb45bc71aac739864a6ef6dc4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849270"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a>tipo de recurso de win32LobAppFileSystemDetection

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém o caminho de arquivo ou pasta para detectar um aplicativo Win32

Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|caminho|Cadeia de caracteres|O caminho de arquivo ou pasta para detectar app Win32 linha de negócios (LoB)|
|fileOrFolderName|Cadeia de caracteres|O nome de arquivo ou pasta para detectar app Win32 linha de negócios (LoB)|
|check32BitOn64System|Booliano|Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits|
|tipo de detecção|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|O tipo de detecção de sistema de arquivos. Os possíveis valores são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.|
|operador|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|O operador para detecção de arquivo ou fodler. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detectionValue|Cadeia de caracteres|O valor de detecção de arquivo ou pasta|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





