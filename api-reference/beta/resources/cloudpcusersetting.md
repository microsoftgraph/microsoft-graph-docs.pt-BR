---
title: Tipo de recurso cloudPcUserSetting
description: Representar uma configuração de usuário de computador na nuvem
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 324d2ba65c82b44595fff366c5d6eb25005c20ef
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993655"
---
# <a name="cloudpcusersetting-resource-type"></a>Tipo de recurso cloudPcUserSetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma configuração de usuário de computador na nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPcUserSettings](../api/virtualendpoint-list-usersettings.md)|[Coleção cloudPcUserSetting](../resources/cloudpcusersetting.md)|Obter uma lista dos [objetos cloudPcUserSetting](../resources/cloudpcusersetting.md) e suas propriedades.|
|[Obter cloudPcUserSetting](../api/cloudpcusersetting-get.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Leia as propriedades e as relações de um [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Criar cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Crie um novo [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Atualizar cloudPcUserSetting](../api/cloudpcusersetting-update.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Atualize as propriedades de [um objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Excluir cloudPcUserSetting](../api/cloudpcusersetting-delete.md)|Nenhum|Exclui um [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[assign](../api/cloudpcusersetting-assign.md)|Nenhum|Atribua [um cloudPcUserSetting a](../resources/cloudpcusersetting.md) grupos de usuários.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a configuração do usuário do computador na nuvem. Somente leitura.|
|displayName|Cadeia de caracteres|O nome da configuração exibido na interface do usuário. |
|localAdminEnabled|Boolean|Indica se a opção de administrador local está habilitada. O valor padrão é `false`. Para habilitar a opção de administrador local, altere a configuração para `true` . |
|selfServiceEnabled|Boolean|Indica se a opção self-service está habilitada. O valor padrão é `false`. Para habilitar a opção self-service, altere a configuração para `true` . |
|lastModifiedDateTime|DateTimeOffset|A última data e hora em que a configuração foi modificada. O tipo Timestamp representa as informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: '2014-01-01T00:00:00Z'. |
|createdDateTime|DateTimeOffset|A data e a hora em que a configuração foi criada. O tipo Timestamp representa as informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: '2014-01-01T00:00:00Z'. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[coleção cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md)|Office 365 e grupos de segurança no Azure AD podem ter um conjunto de configurações de usuário atribuídas.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSetting",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "id": "String (identifier)",
  "displayName": "String",
  "selfServiceEnabled": "Boolean",
  "localAdminEnabled": "Boolean",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```
