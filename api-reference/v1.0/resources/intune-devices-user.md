---
title: Tipo de recurso de usuário
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f5ceecc7122ac9b7a3135c30a7d465eedaf6f34
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60449324"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usuários](../api/intune-devices-user-list.md)|Coleção [user](../resources/intune-devices-user.md)|Listar propriedades e relações de objetos de [user](../resources/intune-devices-user.md).|
|[Obter usuário](../api/intune-devices-user-get.md)|[user](../resources/intune-devices-user.md)|Ler propriedades e relações de objetos de [user](../resources/intune-devices-user.md).|
|[Criar usuário](../api/intune-devices-user-create.md)|[user](../resources/intune-devices-user.md)|Criar um novo objeto de [user](../resources/intune-devices-user.md).|
|[Excluir usuário](../api/intune-devices-user-delete.md)|Nenhum|Excluir [user](../resources/intune-devices-user.md).|
|[Atualizar usuário](../api/intune-devices-user-update.md)|[user](../resources/intune-devices-user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune-devices-user.md).|
|[Ação removeAllDevicesFromManagement](../api/intune-devices-user-removealldevicesfrommanagement.md)|Nenhum|Desativa todos os dispositivos de gerenciamento deste usuário|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|Os dispositivos gerenciados associados ao usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



