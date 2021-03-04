---
title: tipo de recurso directoryRoleTemplate
description: Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório (directoryRole). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 18684434fa7a7b34d82fc98ff7caf34595bc91ef
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440455"
---
# <a name="directoryroletemplate-resource-type"></a>tipo de recurso directoryRoleTemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um modelo de função de diretório. Um modelo de função de diretório especifica os valores de propriedade de uma função de diretório ([directoryRole](directoryrole.md)). Há um modelo de função de diretório associado para cada uma das funções de diretório que podem ser ativadas em um locatário. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST para o ponto de extremidade `/directoryRoles` com a ID do modelo de função de diretório no qual se baseia a função directory especificada no parâmetro **roleTemplateId** da solicitação. Após a conclusão bem-sucedida da solicitação, você pode começar a ler e atribuir membros à função de diretório. **Observação**: Um modelo de função de diretório é exposto para a função de diretório Usuários. A função de diretório Users está implícita e não é visível para os clientes de diretório. Todos os usuários do locatário são atribuídos a essa função pela infraestrutura. A função já está ativada. Não use este modelo.


## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter directoryRoleTemplate](../api/directoryroletemplate-get.md) | [directoryRoleTemplate](directoryroletemplate.md) |Leia as propriedades e os relacionamentos do objeto directoryRoleTemplate.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|A descrição definida para a função de diretório. Somente leitura.|
|displayName|String|O nome de exibição para definir para a função de diretório. Somente leitura. |
|id|String|O identificador exclusivo do modelo. Herdado de [directoryObject](directoryobject.md). Você especifica a **id** do modelo de função do diretório para a propriedade **roleTemplateId** na solicitação POST para ativar um [directoryRole](directoryrole.md) em um locatário. Chave, Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


