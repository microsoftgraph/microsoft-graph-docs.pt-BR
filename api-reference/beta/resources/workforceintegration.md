---
title: Tipo de recurso workforceIntegration
description: Uma instância de integração de força de trabalho com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 12aa4a6ac8fd72f20a0019a95eeb20196b1ed3bf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787650"
---
# <a name="workforceintegration-resource-type"></a>Tipo de recurso workforceIntegration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma instância de integração de força de trabalho com turnos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/workforceintegration-list.md) | [coleção workforceIntegration](workforceintegration.md) | Obter a lista de **objetos workforceIntegration** associados a essa agenda.|
| [Create](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | Crie um novo **objeto workforceIntegration.**|
| [Get](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | Leia as propriedades e as relações de um **objeto workforceIntegration.** |
| [Atualizar](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | Atualizar um **objeto workforceIntegration.** |
| [Delete](../api/workforceintegration-delete.md) | Nenhuma | Excluir um **objeto workforceIntegration.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|apiVersion|Int32|Versão da API para a URL de retorno de chamada. Comece com 1.|
|displayName|String|Nome da integração da força de trabalho.|
|encryption|[workforceIntegrationEncryption](workforceintegrationencryption.md)|O recurso de criptografia de integração de força de trabalho.|
|isActive|Booliano|Indica se essa integração de força de trabalho está ativa e disponível no momento.|
|suporta|cadeia de caracteres| As entidades Shifts suportadas para notificações de alteração síncrona. Os turnos retornarão a url fornecida nas alterações do cliente nessas entidades adicionadas aqui. Por padrão, nenhuma entidade tem suporte para notificações de alteração. Os valores `none` possíveis `shift` são , , , , , , , , `swapRequest` , e `openshift` `openShiftRequest` `userShiftPreferences` `offerShiftRequest` `timeCard` `timeOffReason` `timeOff` `timeOffRequest` `unknownFutureValue` . Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúscula.|
|supportedEntities|cadeia de caracteres| Essa propriedade substituirá **os suportes** em v1.0. Recomendamos que você use essa propriedade em vez de **suporte**. A **propriedade supports** ainda terá suporte na versão beta por enquanto. Os valores `none` possíveis `shift` são , , , , , , , , `swapRequest` , e `openshift` `openShiftRequest` `userShiftPreferences` `offerShiftRequest` `timeCard` `timeOffReason` `timeOff` `timeOffRequest` `unknownFutureValue` . Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúscula.|
|url|Cadeia de caracteres| URL de Integração de Força de Trabalho para retornos de chamada do serviço Shifts.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration"
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


