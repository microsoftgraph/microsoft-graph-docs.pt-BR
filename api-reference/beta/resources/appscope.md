---
title: tipo de recurso appScope
description: Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 23a3d18a8a712ddff8470d91a677f3d0f18dabf2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459332"
---
# <a name="appscope-resource-type"></a>tipo de recurso appScope

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O escopo de uma atribuição de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico. O outro tipo de escopo é o escopo de diretório. Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. 

Isso é empregado na entidade single principal, de escopo único e em várias entidades de escopo múltiplo.

## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| id | string | ID de um contêiner ou recurso específico do aplicativo que representa o escopo da atribuição. Geralmente a ID imutável do recurso. O escopo de uma atribuição determina o conjunto de recursos para o qual a entidade recebeu acesso. Essa propriedade é obrigatória. |
| type | String | Descreve o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo. Fornecido para fins de exibição, de forma que uma interface do usuário possa transmitir ao usuário o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo. Esta propriedade é somente leitura. |
| displayName | cadeia de caracteres | Fornece o nome de exibição do recurso específico do aplicativo representado pelo escopo do aplicativo. Fornecido para fins de exibição, já que appScopeId é geralmente uma ID imutável inalterável e não humanamente legível. Esta propriedade é somente leitura. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appScope"
}-->

```json
{
  "id": "String (identifier)",
  "type": "String",
  "displayName": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->