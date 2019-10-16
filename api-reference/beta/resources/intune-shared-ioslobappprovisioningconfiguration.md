---
title: tipo de recurso iosLobAppProvisioningConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso de configuração de provisionamento do aplicativo LOB do iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58b2b07fdd6562c14b49e781862063c3a9b67aae
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538725"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>tipo de recurso iosLobAppProvisioningConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso de configuração de provisionamento do aplicativo LOB do iOS.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosLobAppProvisioningConfigurations](../api/intune-shared-ioslobappprovisioningconfiguration-list.md)|coleção [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Listar Propriedades e relações dos objetos [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .|
|[Obter iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Leia as propriedades e as relações do objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .|
|[Criar iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Criar um novo objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .|
|[Excluir iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-delete.md)|Nenhum|Exclui [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).|
|[Atualizar iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Atualiza as propriedades de um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .|
|**Apps**|
|[atribuir ação](../api/intune-shared-ioslobappprovisioningconfiguration-assign.md)|Nenhuma|Ainda não documentado|
|**Conjunto de políticas**|
|[ação hasPayloadLinks](../api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md)|coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|expirationDateTime|DateTimeOffset|Data e hora de expiração do perfil opcional.|
|payloadFileName|Cadeia de caracteres|Nome do arquivo de carga (*. mobileprovision | *.xml).|
|payload|Binária|Carga. (Matriz de bytes codificados em UTF8)|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta entidade de configuração de provisionamento do aplicativo LOB iOS.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|description|String|Descrição fornecida pelo administrador da Configuração do dispositivo.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo.|
|versão|Int32|Versão da configuração do dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Apps**|
|groupAssignments|coleção [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|As atribuições de grupo associadas.|
|assignments|coleção [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|As atribuições de grupo associadas para o IosLobAppProvisioningConfiguration.|
|deviceStatuses|coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|A lista de Estados de instalação de dispositivo para esta configuração de aplicativo móvel.|
|userStatuses|Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|A lista de Estados de instalação do usuário para esta configuração de aplicativo móvel.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "binary",
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



