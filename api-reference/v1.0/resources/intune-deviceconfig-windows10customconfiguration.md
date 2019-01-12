---
title: Tipo de recurso windows10CustomConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windows10CustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: baa87da1324527ea2bcc083884323a446e62fa00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952787"
---
# <a name="windows10customconfiguration-resource-type"></a>Tipo de recurso windows10CustomConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windows10CustomConfiguration.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10CustomConfigurations](../api/intune-deviceconfig-windows10customconfiguration-list.md)|Coleção [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md)|Lista propriedades e relações dos objetos [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).|
|[Obter windows10CustomConfiguration](../api/intune-deviceconfig-windows10customconfiguration-get.md)|[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md)|Propriedades de leitura e relações do objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).|
|[Criar windows10CustomConfiguration](../api/intune-deviceconfig-windows10customconfiguration-create.md)|[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md)|Cria um novo objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).|
|[Excluir windows10CustomConfiguration](../api/intune-deviceconfig-windows10customconfiguration-delete.md)|Nenhum|Exclui um [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).|
|[Atualizar windows10CustomConfiguration](../api/intune-deviceconfig-windows10customconfiguration-update.md)|[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md)|Atualiza as propriedades de um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|omaSettings|Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)|Configurações OMA. Essa coleção pode conter um máximo de 1000 elementos.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10CustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "String",
      "description": "String",
      "omaUri": "String",
      "value": 1024
    }
  ]
}
```



