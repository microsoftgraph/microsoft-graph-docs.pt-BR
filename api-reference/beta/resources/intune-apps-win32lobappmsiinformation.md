---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ddb69d3f01c816c592617cb75ed6f9b9877f856
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534483"
---
# <a name="win32lobappmsiinformation-resource-type"></a>tipo de recurso win32LobAppMsiInformation

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades do aplicativo MSI para um aplicativo Win32.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|productCode|String|O código do produto MSI.|
|productVersion|String|A versão do produto MSI.|
|upgradeCode|String|O código de atualização MSI.|
|requiresReboot|Booliano|Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.|
|PackageType|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|O tipo de pacote MSI. Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.|
|productName|Cadeia de caracteres|O nome do produto MSI.|
|publicador|String|O Publicador MSI.|

## <a name="relationships"></a>Relações
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
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```





