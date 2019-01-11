---
title: Tipo de recurso settingStateDeviceSummary
description: Configuração e política de conformidade de dispositivo para um resumo de estado de configuração
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: acd4717901a63963e1e02c3a031bdd1630e84cd1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834423"
---
# <a name="settingstatedevicesummary-resource-type"></a>Tipo de recurso settingStateDeviceSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração e política de conformidade de dispositivo para um resumo de estado de configuração
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar settingStateDeviceSummaries](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Listar propriedades e relações de objetos de [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[Obter settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Ler propriedades e relações de objetos de [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[Criar settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Criar um novo objeto de [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[Excluir settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|Nenhum|Excluir [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[Atualizar settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Atualizar as propriedades de um objeto de [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|settingName|Cadeia de caracteres|Nome da configuração|
|instancePath|Cadeia de caracteres|Nome de InstancePath para a configuração|
|unknownDeviceCount|Int32|Contagem desconhecida de dispositivos para a configuração|
|notApplicableDeviceCount|Int32|Contagem não aplicável ao dispositivo para a configuração|
|compliantDeviceCount|Int32|Contagem de dispositivo em conformidade para a configuração|
|remediatedDeviceCount|Int32|Contagem de dispositivo em conformidade para a configuração|
|nonCompliantDeviceCount|Int32|Contagem de dispositivo sem conformidade para a configuração|
|errorDeviceCount|Int32|Contagem de erros de dispositivo para a configuração|
|conflictDeviceCount|Int32|Contagem de erro de conflito de dispositivo para a configuração|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





