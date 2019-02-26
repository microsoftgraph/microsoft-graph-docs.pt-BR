---
title: tipo de recurso androidOmaCpConfiguration
description: Ao fornecer uma configuração neste perfil, você pode configurar dispositivos Android que oferecem suporte a OMA-CP.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d002568597d5fea2bd895d6d49a7f8cdd886c071
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178084"
---
# <a name="androidomacpconfiguration-resource-type"></a>tipo de recurso androidOmaCpConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer uma configuração neste perfil, você pode configurar dispositivos Android que oferecem suporte a OMA-CP.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidOmaCpConfigurations](../api/intune-deviceconfig-androidomacpconfiguration-list.md)|coleção [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|Listar Propriedades e relações dos objetos [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .|
|[Obter androidOmaCpConfiguration](../api/intune-deviceconfig-androidomacpconfiguration-get.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|Leia as propriedades e as relações do objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .|
|[Criar androidOmaCpConfiguration](../api/intune-deviceconfig-androidomacpconfiguration-create.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|Criar um novo objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .|
|[Excluir androidOmaCpConfiguration](../api/intune-deviceconfig-androidomacpconfiguration-delete.md)|Nenhum|Exclui [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md).|
|[Atualizar androidOmaCpConfiguration](../api/intune-deviceconfig-androidomacpconfiguration-update.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|Atualiza as propriedades de um objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|configurationXml|Binária|XML de configuração que será aplicada ao dispositivo. Quando ele é lido, ele só fornece uma cadeia de caracteres de espaço reservado, pois os dados originais são criptografados e armazenados.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidOmaCpConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "configurationXml": "binary"
}
```




