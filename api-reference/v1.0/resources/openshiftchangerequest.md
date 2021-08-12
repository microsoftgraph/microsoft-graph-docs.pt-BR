---
title: Tipo de recurso openShiftChangeRequest
description: Representa uma solicitação para reivindicar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a6f34e566caa2ff623eb3a66ebf8584b1adeb764dd1e7918bc34f1dbd8455a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229105"
---
# <a name="openshiftchangerequest-resource-type"></a>Tipo de recurso openShiftChangeRequest

Namespace: microsoft.graph

Representa a solicitação para [reivindicar um openShift](../resources/openshift.md) em um [cronograma](../resources/schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/openshiftchangerequest-list.md) | Coleção [de openShiftChangeRequest](openshiftchangerequest.md) | Listar as propriedades e as relações dos **objetos openShiftChangeRequest** em uma equipe. |
| [Criar](../api/openshiftchangerequest-post.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Crie uma instância de um **objeto openShiftChangeRequest.** |
| [Obter](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Leia as propriedades e as relações de um **objeto openShiftChangeRequest.** |
|[Aprovar](../api/openshiftchangerequest-approve.md)|None|Aprovar uma solicitação de alteração de turno aberto.|
|[Declínio](../api/openshiftchangerequest-decline.md)|None| Recusar uma solicitação de alteração de turno aberto.|

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

