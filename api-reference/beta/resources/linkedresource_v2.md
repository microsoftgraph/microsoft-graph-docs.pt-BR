---
title: linkedResource_v2 tipo de recurso
description: Representa um item em um aplicativo parceiro relacionado a um baseTask
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b3c84cf8c4f08800e22841e6928ef85b1162a2e3
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424788"
---
# <a name="linkedresource_v2-resource-type"></a>linkedResource_v2 tipo de recurso

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um item em um aplicativo parceiro relacionado a [um baseTask](./basetask.md). Um exemplo é um email de onde a tarefa foi criada. Um **objeto linkedResource** armazena informações sobre esse aplicativo de origem e permite que você vincule de volta ao item relacionado. Você pode ver **o linkedResource** na exibição de detalhes da tarefa, conforme mostrado.

![Captura de tela mostrando o cartão de recurso vinculado no painel de detalhes da tarefa. O cartão de recurso vinculado mostra Open in Jira, que é o nome do aplicativo parceiro, e Plano de Mídia Social, que é o título do recurso vinculado](/graph/images/todo-linkedresource-taskdetail.png)

Alguns **objetos linkedResource** não estão associados a URLs da Web, nesse caso, a **propriedade webUrl** não é necessária. Por exemplo, o item vinculado pode ser de um aplicativo comercial personalizado ou aplicativo de plataforma nativa, como um aplicativo SMS em um telefone celular. Veja como um **linkedResource** aparece com e sem uma URL.

![Imagem mostrando como o cartão de recurso vinculado com e sem URL é exibido. O cartão de recurso vinculado com URL contém Open with partner application Name enquanto o cartão de recurso vinculado sem URL contém apenas o nome do aplicativo parceiro.](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar linkedResource_v2](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) coleção|Obter uma lista dos objetos [linkedResource_v2](../resources/linkedresource_v2.md) e suas propriedades.|
|[Criar linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Crie um novo [objeto linkedResource_v2.](../resources/linkedresource_v2.md)|
|[Obter linkedResource_v2](../api/linkedresource_v2-get.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Leia as propriedades e as relações de um [linkedResource_v2](../resources/linkedresource_v2.md) objeto.|
|[Atualizar linkedResource_v2](../api/linkedresource_v2-update.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Atualize as propriedades de um [linkedResource_v2](../resources/linkedresource_v2.md) objeto.|
|[Excluir linkedResource_v2](../api/linkedresource_v2-delete.md)|Nenhum|Exclui um [objeto linkedResource_v2.](../resources/linkedresource_v2.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationName|Cadeia de caracteres|Campo indicando o nome do aplicativo da fonte que está enviando **o linkedResource**.|
|displayName|String|Campo que indica o título do **linkedResource**.|
|externalId|Cadeia de caracteres|ID do objeto associado a essa tarefa no sistema de terceiros/parceiro.|
|id|String|ID gerada pelo **servidor para o linkedResource**. Herdado da [entidade](../resources/entity.md).|
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

