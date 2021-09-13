---
title: Tipo de recurso de usuário
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 18955869ac60de15d797ebc79cf7e179673d310d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078781"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar usuários](../api/intune-troubleshooting-user-list.md)|Coleção [user](../resources/intune-troubleshooting-user.md)|Listar propriedades e relações de objetos de [user](../resources/intune-troubleshooting-user.md).|
|[Obter usuário](../api/intune-troubleshooting-user-get.md)|[user](../resources/intune-troubleshooting-user.md)|Ler propriedades e relações de objetos de [user](../resources/intune-troubleshooting-user.md).|
|[Criar usuário](../api/intune-troubleshooting-user-create.md)|[user](../resources/intune-troubleshooting-user.md)|Criar um novo objeto de [user](../resources/intune-troubleshooting-user.md).|
|[Excluir usuário](../api/intune-troubleshooting-user-delete.md)|Nenhum|Excluir [user](../resources/intune-troubleshooting-user.md).|
|[Atualizar usuário](../api/intune-troubleshooting-user-update.md)|[user](../resources/intune-troubleshooting-user.md)|Atualizar as propriedades de um objeto de [user](../resources/intune-troubleshooting-user.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do usuário.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceManagementTroubleshootingEvents|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|A lista de eventos de solução de problemas desse usuário.|

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




