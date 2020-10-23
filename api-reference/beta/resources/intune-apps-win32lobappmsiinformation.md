---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f80e41eec3b2e6b494d076029a5408267da65595
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732654"
---
# <a name="win32lobappmsiinformation-resource-type"></a>tipo de recurso win32LobAppMsiInformation

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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





