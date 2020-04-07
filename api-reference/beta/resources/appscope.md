---
title: tipo de recurso appScope
description: 'O escopo de uma atribuição de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico. O outro tipo de escopo é o escopo de diretório. Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a996b219df124ac0c287ed4ed32658584acb6ac
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160349"
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
| displayName | string | Fornece o nome de exibição do recurso específico do aplicativo representado pelo escopo do aplicativo. Fornecido para fins de exibição, já que appScopeId é geralmente uma ID imutável inalterável e não humanamente legível. Esta propriedade é somente leitura. |

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