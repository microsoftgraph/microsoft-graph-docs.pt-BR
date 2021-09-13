---
title: Tipo de recurso appScope
description: Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 1cb198e26bae9bf41a63bb834564245c77192863
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59110484"
---
# <a name="appscope-resource-type"></a>Tipo de recurso appScope

O escopo de uma atribuição de função determina o conjunto de recursos para os quais a entidade recebeu acesso. Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico, ao contrário dos escopos de diretório que são escopos compartilhados armazenados no diretório e compreendidos por vários aplicativos.

Isso pode estar nos seguintes cenários principais e de escopo:
+ Uma única entidade principal e um único escopo
+ Várias entidades principais e vários escopos.
    
Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos
Nenhum(a)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| displayName | cadeia de caracteres | Fornece o nome de exibição do recurso específico do aplicativo representado pelo escopo do aplicativo. Fornecido para fins de exibição, já que appScopeId geralmente é uma id imutável, não acessível para humanos. Somente leitura. |
| id | cadeia de caracteres | Identificador de um contêiner ou recurso específico do aplicativo que representa o escopo da atribuição. Geralmente, a ID imutável do recurso. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Obrigatório. |
| tipo | Cadeia de caracteres | Descreve o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo. Fornecido para fins de exibição, para que uma interface do usuário possa transmitir ao usuário o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo. Somente leitura. |

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
