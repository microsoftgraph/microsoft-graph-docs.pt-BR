---
title: tipo de recurso linkedResource
description: Representa a fonte do todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3cbfaa0bf809a1996fe7a7c7df7014324406bcf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058106"
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
|[Excluir linkedResource](../api/linkedresource-delete.md)|Nenhum|Exclui um objeto [linkedResource](../resources/linkedresource.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationName|Cadeia de caracteres|Campo que indica o nome do aplicativo de origem que está enviando o **linkedResource**.|
|displayName|Cadeia de caracteres|Campo que indica o título do **linkedResource**.|
|externalId|Cadeia de caracteres|ID do objeto que está associado a essa tarefa no sistema de parceiros ou de terceiros.|
|id|Cadeia de caracteres|ID gerada pelo servidor para o **linkedResource**. Herdado de [entidade](../resources/entity.md).|
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



