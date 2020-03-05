---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 92ff70c8b1bbf63ce6fd81321282a0f61f4accc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490690"
---
# <a name="win32lobappmsiinformation-resource-type"></a>tipo de recurso win32LobAppMsiInformation

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades do aplicativo MSI para um aplicativo Win32.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|productCode|String|O código do produto MSI.|
|productVersion|String|A versão do produto MSI.|
|upgradeCode|String|O código de atualização MSI.|
|requiresReboot|Boolean|Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.|
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



