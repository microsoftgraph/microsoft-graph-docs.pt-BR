---
title: Tipo de recurso softwareUpdateStatusSummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3f70e091bc39b8591d59c2904a1e9ad743fcffa1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758796"
---
# <a name="softwareupdatestatussummary-resource-type"></a>Tipo de recurso softwareUpdateStatusSummary

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter softwareUpdateStatusSummary](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Ler propriedades e relações de objetos de [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).|
|[Atualizar softwareUpdateStatusSummary](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Atualizar as propriedades de um objeto de [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|String|O nome da política.|
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




