---
title: Tipo de recurso workforceIntegration
description: Uma instância de integração de força de trabalho com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c1d5665f289215a7a5ffb8721976ec9b93289785804be0b49d40c79cd5ad963d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163632"
---
# <a name="workforceintegration-resource-type"></a>Tipo de recurso workforceIntegration

Namespace: microsoft.graph

Uma instância de integração de força de trabalho com turnos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | Crie um novo **objeto workforceIntegration.**|
| [List](../api/workforceintegration-list.md) | [coleção workforceIntegration](workforceintegration.md) | Obter a lista de **objetos workforceIntegration** associados a essa agenda.|
| [Obter](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | Leia as propriedades e as relações de um **objeto workforceIntegration.** |
| [Atualizar](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | Atualizar um **objeto workforceIntegration.** |
| [Delete](../api/workforceintegration-delete.md) | None | Excluir um **objeto workforceIntegration.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|apiVersion|Int32|Versão da API para a URL de retorno de chamada. Comece com 1.|
|displayName|Cadeia de caracteres|Nome da integração da força de trabalho.|
|encryption|[workforceIntegrationEncryption](workforceintegrationencryption.md)|O recurso de criptografia de integração de força de trabalho.|
|isActive|Booliano|Indica se essa integração de força de trabalho está ativa e disponível no momento.|
|supportedEntities|workforceIntegrationSupportedEntities | As entidades Shifts suportadas para notificações de alteração síncrona. Os turnos retornarão a url fornecida nas alterações do cliente nessas entidades adicionadas aqui. Por padrão, nenhuma entidade tem suporte para notificações de alteração. Os valores possíveis são: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openshift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|
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

