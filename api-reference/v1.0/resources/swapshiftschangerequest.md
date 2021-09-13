---
title: Tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar um turno com outro usuário na equipe.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 396e4d9dd08044bd726b9e6f85ed808065ec37da
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134448"
---
# <a name="swapshiftschangerequest-resource-type"></a>Tipo de recurso swapShiftsChangeRequest

Namespace: microsoft.graph

Representa um tipo de solicitação de turno para trocar um [turno](../resources/shift.md) com outro usuário na [equipe.](../resources/team.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/swapshiftschangerequest-list.md) | Coleção [de swapShiftsChangeRequest](swapshiftschangerequest.md) | Listar as propriedades e as relações dos **objetos swapShiftsChangeRequest** em uma equipe. |
| [Criar](../api/swapshiftschangerequest-post.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Crie uma instância de um **objeto swapShiftsChangeRequest.** |
| [Obter](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Leia as propriedades e as relações de um **objeto swapShiftsChangeRequest.** |
|[Aprovar](../api/swapshiftschangerequest-approve.md)|Nenhum(a)|Aprovar um **swapShiftsChangeRequest**. |
|[Declínio](../api/swapshiftschangerequest-decline.md)|Nenhum(a)|Recusar um **swapShiftsChangeRequest**.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientShiftId|Cadeia de caracteres|ShiftId para o usuário destinatário com o qual a solicitação deve ser trocada.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
}-->

```json
{
  "recipientShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftsChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

