---
title: Tipo de recurso hardwareConfigurationUserState
description: Contém propriedades para o estado do usuário da configuração de hardware
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ecd964d5c5f2d18ffef71e04ebba40de8f3759ff
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345376"
---
# <a name="hardwareconfigurationuserstate-resource-type"></a>Tipo de recurso hardwareConfigurationUserState

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado do usuário da configuração de hardware

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar hardwareConfigurationUserStates](../api/intune-deviceconfig-hardwareconfigurationuserstate-list.md)|[Coleção hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Listar propriedades e relações dos [objetos hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|
|[Obter hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-get.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Ler propriedades e relações do [objeto hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|
|[Criar hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-create.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Crie um novo [objeto hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|
|[Excluir hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-delete.md)|Nenhum|Exclui [um hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md).|
|[Atualizar hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-update.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Atualize as propriedades de [um objeto hardwareConfigurationUserState.](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de estado do usuário do script de configuração de hardware. Essa propriedade é somente leitura.|
|upn|String|Nome UPN|
|userEmail|Cadeia de caracteres|Endereço de Email do Usuário|
|userName|Cadeia de caracteres|Nome de usuário|
|lastStateUpdateDateTime|DateTimeOffset|Last timestamp when the hardware configuration executed|
|successfulDeviceCount|Int32|Contagem de dispositivos de sucesso para um usuário específico|
|failedDeviceCount|Int32|Contagem de dispositivos com falha para um usuário específico|
|pendingDeviceCount|Int32|Contagem de dispositivos pendente para um usuário específico.|
|errorDeviceCount|Int32|Contagem de dispositivos de erro para usuário específico.|
|notApplicableDeviceCount|Int32|Contagem de dispositivos não aplicável para um usuário específico.|
|unknownDeviceCount|Int32|Contagem de dispositivos desconhecidos para usuários específicos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "id": "String (identifier)",
  "upn": "String",
  "userEmail": "String",
  "userName": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "successfulDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




