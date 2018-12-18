---
title: tipo de recurso de win32LobAppFileSystemDetection
description: Contém o caminho de arquivo ou pasta para detectar um aplicativo Win32
author: tfitzmac
ms.openlocfilehash: 26d65c8a1fcf70032c780b3e6e00a198a8ff2c30
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306871"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a>tipo de recurso de win32LobAppFileSystemDetection

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém o caminho de arquivo ou pasta para detectar um aplicativo Win32

Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|caminho|String|O caminho de arquivo ou pasta para detectar app Win32 linha de negócios (LoB)|
|fileOrFolderName|String|O nome de arquivo ou pasta para detectar app Win32 linha de negócios (LoB)|
|check32BitOn64System|Boolean|Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits|
|tipo de detecção|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|O tipo de detecção de sistema de arquivos. Os possíveis valores são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.|
|operador|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|O operador para detecção de arquivo ou fodler. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detectionValue|String|O valor de detecção de arquivo ou pasta|

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





