---
title: Tipo de recurso softwareUpdateStatusSummary
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c297c61528f50aea023109f3a71ff877343d8ef3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838892"
---
# <a name="softwareupdatestatussummary-resource-type"></a>Tipo de recurso softwareUpdateStatusSummary

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter softwareUpdateStatusSummary](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Ler propriedades e relações de objetos de [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).|
|[Atualizar softwareUpdateStatusSummary](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Atualizar as propriedades de um objeto de [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|O nome da política.|
|compliantDeviceCount|Int32|Número de dispositivos em conformidade.|
|nonCompliantDeviceCount|Int32|Número de dispositivos sem conformidade.|
|remediatedDeviceCount|Int32|Número de dispositivos corrigidos.|
|errorDeviceCount|Int32|Número de dispositivos com erro.|
|unknownDeviceCount|Int32|Número de dispositivos desconhecidos.|
|conflictDeviceCount|Int32|Número de dispositivos em conflito.|
|notApplicableDeviceCount|Int32|Número de dispositivos não aplicáveis.|
|compliantUserCount|Int32|Número de usuários em conformidade.|
|nonCompliantUserCount|Int32|Número de usuários em não conformidade.|
|remediatedUserCount|Int32|Número de usuários corrigidos.|
|errorUserCount|Int32|Número de usuários com erro.|
|unknownUserCount|Int32|Número de usuários desconhecidos.|
|conflictUserCount|Int32|Número de usuários com conflitos.|
|notApplicableUserCount|Int32|Número de usuários não aplicáveis.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```



