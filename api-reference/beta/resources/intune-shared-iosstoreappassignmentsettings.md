---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4249a0c8ef6959f779b93dba4c30947e411890d4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788258"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a>Tipo de recurso iosStoreAppAssignmentSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.


Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|vpnConfigurationId|Cadeia de caracteres|A identificação de configuração da VPN a aplicar neste aplicativo.|
|**Aplicativos**|
|uninstallOnDeviceRemoval|Boleano|Se deve ou não desinstalar o aplicativo quando o dispositivo for removido do Intune.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



