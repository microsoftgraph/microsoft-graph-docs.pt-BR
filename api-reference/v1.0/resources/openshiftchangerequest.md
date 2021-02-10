---
title: Tipo de recurso openShiftChangeRequest
description: Representa uma solicitação para reivindicar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b427d7914d95aaed794734bbbb39fa3eb139d06a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158678"
---
# <a name="openshiftchangerequest-resource-type"></a>Tipo de recurso openShiftChangeRequest

Namespace: microsoft.graph

Representa a solicitação para [reivindicar um openShift](../resources/openshift.md) em um [cronograma](../resources/schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/openshiftchangerequest-list.md) | Coleção de [openShiftChangeRequest](openshiftchangerequest.md) | Listar as propriedades e os relacionamentos dos **objetos openShiftChangeRequest** em uma equipe. |
| [Criar](../api/openshiftchangerequest-post.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Crie uma instância de um **objeto openShiftChangeRequest.** |
| [Get](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Leia as propriedades e os relacionamentos de um **objeto openShiftChangeRequest.** |
|[Aprovar](../api/openshiftchangerequest-approve.md)|Nenhum|Aprovar uma solicitação de alteração de turno aberto.|
|[Recusar](../api/openshiftchangerequest-decline.md)|Nenhum| Recusar uma solicitação de alteração de turno aberto.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|openShiftId|Cadeia de caracteres| ID do turno aberto.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
}-->

```json
{
  "openShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

