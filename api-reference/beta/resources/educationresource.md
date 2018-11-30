---
title: tipo de recurso de educationResource
description: Uma superclasse para todos os objetos de recursos no sistema. Um recurso é associado a uma **atribuição** e/ou o **envio**, que representa o objeto de aprendizado que está sendo
ms.openlocfilehash: b7e64a946992bb0b43c5bfe50e8d92b5f7176856
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038549"
---
# <a name="educationresource-resource-type"></a>tipo de recurso de educationResource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma superclasse para todos os objetos de recursos no sistema. Um recurso é associado a uma **atribuição** e/ou o **envio**, que representa o objeto de aprendizado que está sendo atribuídas ou fornecidos. Você não pode instanciar um recurso diretamente; Você deve fazer uma subclasse que representará o tipo de recurso que está sendo usado.

Este recurso armazena as propriedades comuns em todos os tipos de recurso.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Quem criou o recurso.|
|createdDateTime|Momento em que o recurso foi criado.  DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|displayName|String|Exibe o nome do recurso.|
|lastModifiedBy|[identitySet](identityset.md)|Quem foi o último usuário para modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no tempo de última modificação do recurso.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->