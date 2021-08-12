---
title: Tipo de recurso de usuário
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 183c751ace228293cb20c0e459e8de75e6fb143d7e4f374e35ee2cf8a3ad884a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189518"
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




