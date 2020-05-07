---
title: tipo de recurso workforceIntegration
description: Uma instância de uma integração de força de funcionários com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fb78761105138aead9a940db23305d7a0d41f92e
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154154"
---
# <a name="workforceintegration-resource-type"></a>tipo de recurso workforceIntegration

Namespace: microsoft.graph

Uma instância de uma integração de força de funcionários com turnos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | Criar um novo objeto **workforceIntegration** .|
| [List](../api/workforceintegration-list.md) | coleção [workforceIntegration](workforceintegration.md) | Obtenha a lista de objetos **workforceIntegration** associados a esse cronograma.|
| [Get](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | Leia as propriedades e os relacionamentos de um objeto **workforceIntegration** . |
| [Update](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | Atualizar um objeto **workforceIntegration** . |
| [Delete](../api/workforceintegration-delete.md) | None | Excluir um objeto **workforceIntegration** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|apiVersion|Int32|Versão da API para a URL de retorno de chamada. Comece com 1.|
|displayName|Cadeia de caracteres|Nome da integração da força de funcionários.|
|encripta|[workforceIntegrationEncryption](workforceintegrationencryption.md)|O recurso de criptografia de integração da força de funcionários.|
|isActive|Booliano|Indica se a integração da força de trabalho está ativa e disponível atualmente.|
|supportedEntities|string| As entidades de alternância têm suporte para notificações de alteração síncrona. Os turnos farão uma chamada de volta para a URL fornecida nas alterações de cliente nas entidades adicionadas aqui. Por padrão, nenhuma entidade tem suporte para notificações de alteração. Os valores possíveis são `none`: `shift`, `swapRequest`, `openshift`, `openShiftRequest`,,`userShiftPreferences`|
|url|Cadeia de caracteres| URL de integração de força de obra para retornos de chamada do serviço de turnos.|

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
