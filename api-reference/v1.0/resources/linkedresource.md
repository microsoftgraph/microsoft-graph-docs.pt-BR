---
title: Tipo de recurso linkedResource
description: Representa a origem do todoTask
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: dfc5e05403c93f07f48c010b8d7233543021f52c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036148"
---
# <a name="linkedresource-resource-type"></a>Tipo de recurso linkedResource

Namespace: microsoft.graph


Representa um item em um aplicativo parceiro relacionado a [um todoTask](./todotask.md). Um exemplo é um email de onde a tarefa foi criada. Um **objeto linkedResource** armazena informações sobre esse aplicativo de origem e permite que você vincule de volta ao item relacionado. Você pode ver **o linkedResource** na exibição de detalhes da tarefa, conforme mostrado.

![Recurso vinculado no painel de detalhes da tarefa](/graph/images/todo-linkedresource-taskdetail.png)

Alguns **objetos linkedResource** não estão associados a URLs da Web, nesse caso, a **propriedade webUrl** não é necessária. Por exemplo, o item vinculado pode ser de um aplicativo comercial personalizado ou aplicativo de plataforma nativa, como um aplicativo SMS em um telefone celular. Veja como um **linkedResource** aparece com e sem uma URL.

![Recurso vinculado com e sem URL](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar linkedResources](../api/todotask-list-linkedresources.md)|[Coleção linkedResource](../resources/linkedresource.md)|Obter o linkedResources da propriedade de navegação linkedResources.|
|[Criar linkedResource](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|Crie um novo objeto linkedResources.|
|[Obter linkedResource](../api/linkedresource-get.md)|[linkedResource](../resources/linkedresource.md)|Leia as propriedades e as relações de um [objeto linkedResource.](../resources/linkedresource.md)|
|[Atualizar linkedResource](../api/linkedresource-update.md)|[linkedResource](../resources/linkedresource.md)|Atualize as propriedades de um [objeto linkedResource.](../resources/linkedresource.md)|
|[Excluir linkedResource](../api/linkedresource-delete.md)|None|Exclui um [objeto linkedResource.](../resources/linkedresource.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationName|Cadeia de caracteres|Campo indicando o nome do aplicativo da fonte que está enviando **o linkedResource**.|
|displayName|String|Campo que indica o título do **linkedResource**.|
|externalId|Cadeia de caracteres|ID do objeto associado a essa tarefa no sistema de terceiros/parceiro.|
|id|Cadeia de caracteres|ID gerada pelo **servidor para o linkedResource**. Herdado da [entidade](../resources/entity.md).|
|webUrl|String|Link profundo para **o linkedResource**.|

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



