---
title: tipo de recurso de win32LobAppMsiInformation
description: Contém propriedades de app MSI para um aplicativo Win32.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04972e9e7fa909c220fe55ca6337be3ac44138ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967872"
---
# <a name="win32lobappmsiinformation-resource-type"></a>tipo de recurso de win32LobAppMsiInformation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades de app MSI para um aplicativo Win32.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|productCode|Cadeia de caracteres|O código do produto MSI.|
|productVersion|Cadeia de caracteres|A versão MSI do produto.|
|upgradeCode|Cadeia de caracteres|O código de atualização de MSI.|
|requiresReboot|Booliano|Se o aplicativo MSI requer a máquina reinicie para concluir a instalação.|
|tipo de pacote|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|O tipo de pacote MSI. Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.|

## <a name="relationships"></a>Relacionamentos
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String"
}
```





