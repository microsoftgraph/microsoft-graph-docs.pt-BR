---
title: Tipo de recurso windowsManagementAppHealthState
description: Windows estado de saúde do aplicativo de gerenciamento.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 885827482bcf24bfe6b90c2feb564190e004975a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040033"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>Tipo de recurso windowsManagementAppHealthState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows estado de saúde do aplicativo de gerenciamento.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[coleção windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Listar propriedades e relações dos [objetos windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)|
|[Obter windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Leia propriedades e relações do [objeto windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)|
|[Criar windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Crie um novo [objeto windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)|
|[Excluir windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|Nenhum|Exclui um [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).|
|[Atualizar windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Atualize as propriedades de um [objeto windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para o estado de Windows de saúde do aplicativo de gerenciamento. Essa propriedade é somente leitura.|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Windows estado de saúde do aplicativo de gerenciamento. Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|Cadeia de Caracteres|Windows versão instalada do aplicativo de gerenciamento.|
|lastCheckInDateTime|DateTimeOffset|Windows aplicativo de gerenciamento última hora de check-in.|
|deviceName|String|Nome do dispositivo no qual o Windows de gerenciamento está instalado.|
|deviceOSVersion|Cadeia de Caracteres|Windows 10 Versão do sistema operacional do dispositivo no qual o Windows de gerenciamento está instalado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```



