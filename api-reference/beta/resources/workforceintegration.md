---
title: tipo de recurso workforceIntegration
description: Uma instância de uma integração de força de funcionários com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e836a4346fe5e31f39c1f6383acbf78530ae9e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519082"
---
# <a name="workforceintegration-resource-type"></a>tipo de recurso workforceIntegration

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma instância de uma integração de força de funcionários com turnos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | Leia as propriedades e os relacionamentos de um objeto **workforceIntegration** . |
| [Update](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | Atualizar um objeto **workforceIntegration** . |
| [Delete](../api/workforceintegration-delete.md) | None | Excluir um objeto **workforceIntegration** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|apiVersion|Int32|Versão da API para a URL de retorno de chamada. Comece com 1.|
|displayName|String|Nome da integração da força de funcionários.|
|encripta|[workforceIntegrationEncryption](workforceintegrationencryption.md)|O recurso de criptografia de integração da força de funcionários.|
|isActive|Boolean|Indica se a integração da força de trabalho está ativa e disponível atualmente.|
|compatível|string| Os valores possíveis são `none`: `shift`, `swapRequest`, `openshift`, `openShiftRequest`,,`userShiftPreferences`|
|url|Cadeia de caracteres| URL de integração de força de obra para retornos de chamada do serviço de turno.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration",
  "baseType": ""
}-->

```json
{
  "apiVersion": 1024,
  "displayName": "String",
  "encryption": {"@odata.type": "microsoft.graph.workforceIntegrationEncryption"},
  "isActive": true,
  "supports": "string",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
