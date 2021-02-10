---
title: Tipo de recurso workforceIntegration
description: Uma instância de uma integração da força de trabalho com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 637e18d2751ee528331771f11f41fc893770ad09
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158930"
---
# <a name="workforceintegration-resource-type"></a>Tipo de recurso workforceIntegration

Namespace: microsoft.graph

Uma instância de uma integração da força de trabalho com turnos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | Crie um novo **objeto workforceIntegration.**|
| [Lista](../api/workforceintegration-list.md) | [coleção workforceIntegration](workforceintegration.md) | Obter a lista de **objetos workforceIntegration** associados a este cronograma.|
| [Get](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | Leia as propriedades e os relacionamentos de um **objeto workforceIntegration.** |
| [Update](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | Atualize **um objeto workforceIntegration.** |
| [Delete](../api/workforceintegration-delete.md) | Nenhum | Exclua **um objeto workforceIntegration.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|apiVersion|Int32|Versão da API para a URL de retorno de chamada. Comece com 1.|
|displayName|Cadeia de caracteres|Nome da integração da força de trabalho.|
|criptografia|[workforceIntegrationEncryption](workforceintegrationencryption.md)|O recurso de criptografia de integração da força de trabalho.|
|isActive|Booliano|Indica se essa integração de força de trabalho está ativa e disponível no momento.|
|supportedEntities|string| As entidades Shifts com suporte para notificações de alteração síncrona. Os turnos fazem uma chamada de volta para a URL fornecida nas alterações do cliente nessas entidades adicionadas aqui. Por padrão, nenhuma entidade tem suporte para notificações de alteração. Os valores possíveis `none` são: `shift` , , , `swapRequest` `openshift` , `openShiftRequest``userShiftPreferences`|
|url|Cadeia de caracteres| URL de integração da força de trabalho para retornos de chamada do serviço Shifts.|

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
  "supportedEntities": "string",
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

