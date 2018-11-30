---
title: tipo de recurso de programControlType
description: 'No Windows Azure AD access analisa o recurso, o tipo de controle do programa é usado quando a associação de um controle a um programa, para indicar o tipo da revisão do acesso de controle se destina.  '
ms.openlocfilehash: 8fc406648d8f8c943920507a5734f47d2add1b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037120"
---
# <a name="programcontroltype-resource-type"></a>tipo de recurso de programControlType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o tipo de controle do programa é usado quando a associação de um controle a um programa, para indicar o tipo de revisão de acesso, que o controle se destina.  

Os objetos de tipo de controle do programa são gerados automaticamente quando o onboards administrador global locatário para usar o access revisa o recurso.  Não há tipos de controle de programa adicionais podem ser criados.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](programcontroltype.md)| Lista os tipos de controle do programa. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                     |`String`                | O identificador atribuído pelo recurso do tipo de controle de programa                                      |
| `displayName`            |`String`                | O nome do tipo de controle de programa                                                             |


## <a name="relationships"></a>Relações

Nenhum.


## <a name="see-also"></a>Ver também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicione um programControl a um programa.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
