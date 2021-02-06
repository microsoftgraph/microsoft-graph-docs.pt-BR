---
title: Tipo de recurso appScope
description: Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: de49425bddc5905d1b1bf17afeb5fb7c5363038c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136007"
---
# <a name="appscope-resource-type"></a>Tipo de recurso appScope

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O escopo de uma atribuição de função determina o conjunto de recursos para os quais a entidade de serviço recebeu acesso. Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico. O outro tipo de escopo é o escopo de diretório. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. 

Isso é empregado tanto na entidade principal única, quanto na entidade de escopo único e em várias entidades de escopo principal e múltipla.

## <a name="methods"></a>Métodos
Nenhuma

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| id | string | ID de um contêiner ou recurso específico do aplicativo que representa o escopo da atribuição. Geralmente, a ID imutável do recurso. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade de serviço recebeu acesso. Essa propriedade é necessária. |
| type | String | Descreve o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo. Fornecido para fins de exibição, para que uma interface do usuário possa transmitir ao usuário o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo. Essa propriedade é somente leitura. |
| displayName | string | Fornece o nome de exibição do recurso específico do aplicativo representado pelo escopo do aplicativo. Fornecido para fins de exibição, uma vez que appScopeId geralmente é uma ID imutável, não aceitável de leitura humana. Essa propriedade é somente leitura. |

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

