---
title: tipo de recurso linkedResource
description: Representa a fonte do todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 70303742db1dabb866585be7099cb222f8a428bd
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797184"
---
# <a name="linkedresource-resource-type"></a>tipo de recurso linkedResource

Namespace: microsoft.graph


Representa um item em um aplicativo parceiro relacionado a um [todoTask](./todotask.md). Um exemplo é um email de onde a tarefa foi criada. Um objeto **linkedResource** armazena informações sobre esse aplicativo de origem e permite que você vincule novamente ao item relacionado. Você pode ver o **linkedResource** no modo de exibição detalhes da tarefa, conforme mostrado.

![Recurso vinculado no painel de detalhes da tarefa](/graph/images/todo-linkedresource-taskdetail.png)

Alguns objetos **linkedResource** não estão associados a qualquer URL da Web, e nesse caso, a propriedade **WebUrl** não é necessária. Por exemplo, o item vinculado pode ser de um aplicativo de negócios personalizado ou de uma plataforma nativa, como um aplicativo do SMS em um telefone celular. Veja como um **linkedResource** aparece com e sem uma URL.

![Recurso vinculado com e sem URL](/graph/images/todo-linkedresource.png)

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
|applicationName|Cadeia de caracteres|Campo que indica o nome do aplicativo de origem que está enviando o **linkedResource** .|
|displayName|String|Campo que indica o título do **linkedResource** .|
|externalId|Cadeia de caracteres|ID do objeto que está associado a essa tarefa no sistema de parceiros ou de terceiros.|
|id|String|ID gerada pelo servidor para o **linkedResource** . Herdado de [entidade](../resources/entity.md).|
|webUrl|String|Link profundo para o **linkedResource** .|

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



