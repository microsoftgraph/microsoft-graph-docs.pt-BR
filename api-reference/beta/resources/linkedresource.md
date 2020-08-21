---
title: tipo de recurso linkedResource
description: Representa a fonte do todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a386cd8ed714a6f7127ea0a872a4170997bb8b9
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849861"
---
# <a name="linkedresource-resource-type"></a>tipo de recurso linkedResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um item em um aplicativo parceiro relacionado a um [todoTask](./todotask.md). Um exemplo é um email que criou a tarefa. Um objeto **linkedResource** armazena informações sobre esse aplicativo de origem e permite que você vincule novamente ao item relacionado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar linkedResources](../api/todotask-list-linkedresources.md)|coleção [linkedResource](../resources/linkedresource.md)|Obtenha o linkedResources da propriedade de navegação linkedResources.|
|[Criar linkedResource](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|Criar um novo objeto linkedResources.|
|[Obter linkedResource](../api/linkedresource-get.md)|[linkedResource](../resources/linkedresource.md)|Leia as propriedades e os relacionamentos de um objeto [linkedResource](../resources/linkedresource.md) .|
|[Atualizar linkedResource](../api/linkedresource-update.md)|[linkedResource](../resources/linkedresource.md)|Atualiza as propriedades de um objeto [linkedResource](../resources/linkedresource.md) .|
|[Excluir linkedResource](../api/linkedresource-delete.md)|Nenhuma|Exclui um objeto [linkedResource](../resources/linkedresource.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationName|Cadeia de caracteres|Campo que indica o nome do aplicativo de origem que está enviando o **linkedResource**.|
|displayName|String|Campo que indica o título do **linkedResource**.|
|externalId|Cadeia de caracteres|ID do objeto que está associado a essa tarefa no sistema de parceiros ou de terceiros.|
|id|String|ID gerada pelo servidor para o **linkedResource**. Herdado de [entidade](../resources/entity.md).|
|webUrl|String|Link profundo para o **linkedResource**.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "String (identifier)",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String"
}
```

