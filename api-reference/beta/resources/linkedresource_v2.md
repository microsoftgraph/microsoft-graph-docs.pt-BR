---
title: linkedResource_v2 tipo de recurso
description: Representa um item em um aplicativo de parceiro relacionado a uma baseTask
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 720fd4e10664f4f83a0c050d6b4838d68e3f59c7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820996"
---
# <a name="linkedresource_v2-resource-type-deprecated"></a>linkedResource_v2 tipo de recurso (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Representa um item em um aplicativo parceiro relacionado a uma [baseTask](./basetask.md). Um exemplo é um email de onde a tarefa foi criada. Um **objeto linkedResource** armazena informações sobre esse aplicativo de origem e permite que você vincule de volta ao item relacionado. Você pode ver o **linkedResource** na exibição de detalhes da tarefa, conforme mostrado.

![Captura de tela mostrando o cartão de recurso vinculado no painel de detalhes da tarefa. O cartão de recurso vinculado mostra Abrir no Jira, que é o nome do aplicativo parceiro, e o Plano de Mídia Social, que é o título do recurso vinculado](/graph/images/todo-linkedresource-taskdetail.png)

Alguns **objetos linkedResource** não estão associados a urLs da Web, nesse caso, a propriedade **webUrl** não é necessária. Por exemplo, o item vinculado pode ser de um aplicativo de negócios personalizado ou aplicativo de plataforma nativa, como um SMS em um telefone celular. Veja como um **linkedResource aparece** com e sem uma URL.

![Imagem mostrando como o cartão de recurso vinculado com e sem URL é exibido. O cartão de recurso vinculado com URL contém Abrir com o nome do aplicativo parceiro enquanto o cartão de recurso vinculado sem URL contém apenas o nome do aplicativo parceiro.](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar linkedResource_v2](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) coleção|Obtenha uma lista dos [objetos linkedResource_v2](../resources/linkedresource_v2.md) e suas propriedades.|
|[Criar linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Crie um novo [linkedResource_v2](../resources/linkedresource_v2.md) objeto.|
|[Obter linkedResource_v2](../api/linkedresource_v2-get.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Leia as propriedades e as relações de um [linkedResource_v2](../resources/linkedresource_v2.md) objeto.|
|[Atualizar linkedResource_v2](../api/linkedresource_v2-update.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Atualize as propriedades de [um linkedResource_v2](../resources/linkedresource_v2.md) objeto.|
|[Excluir linkedResource_v2](../api/linkedresource_v2-delete.md)|Nenhum|Exclui um [linkedResource_v2](../resources/linkedresource_v2.md) objeto.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationName|Cadeia de caracteres|Campo que indica o nome do aplicativo da origem que está enviando **o linkedResource**.|
|displayName|Cadeia de caracteres|Campo que indica o título do **linkedResource**.|
|externalId|Cadeia de caracteres|ID do objeto associado a essa tarefa no sistema de terceiros/parceiro.|
|id|String|ID gerada pelo servidor para **o linkedResource**. Herdado da [entidade](../resources/entity.md).|
|webUrl|String|Link profundo para **o linkedResource**.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource_v2",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource_v2",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)"
}
```

