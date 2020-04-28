---
title: tipo de recurso activityBasedTimeoutPolicy
description: Representa uma política que pode controlar o tempo limite de ociosidade para sessões da Web para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb2f62f2d871afdf035bd264c40af0e521e30b31
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917331"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a>tipo de recurso activityBasedTimeoutPolicy

Namespace: microsoft.graph

Representa uma política que pode controlar o tempo limite de ociosidade para sessões da Web para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade. Os aplicativos impõem a desconexão automática após um período de inatividade. Esse tipo de política só pode ser aplicado no nível da organização (Configurando **isOrganizationDefault** a propriedade isOrganizationDefault `true`para).

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar activityBasedTimeoutPolicies](../api/activitybasedtimeoutpolicy-list.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Ler propriedades e relações de objetos activityBasedTimeoutPolicy. |
| [Criar activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Criar um objeto activityBasedTimeoutPolicy. |
| [Obter activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-get.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Ler propriedades e relações de um objeto activityBasedTimeoutPolicy. |
| [Atualizar activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-update.md) | Nenhum | Atualize um objeto activityBasedTimeoutPolicy. |
| [Excluir activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-delete.md) | Nenhum | Excluir um objeto activityBasedTimeoutPolicy. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo da política. Somente leitura.|
|definir|Coleção de cadeias de caracteres| Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política. Veja mais detalhes sobre o esquema JSON para esta propriedade. Obrigatório.|
|description|String| Descrição da política.|
|displayName|Cadeia de caracteres| Nome para exibição dessa política. Obrigatório.|
|isOrganizationDefault|Boolean|Se definido como true, ativa esta política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão. Opcional, o valor padrão é false.|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a>Propriedades de uma definição de política de tempo limite baseada em atividade
As propriedades abaixo formam o objeto JSON que representa uma política de tempo limite baseada na atividade. Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** . Um exemplo é mostrado abaixo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

>**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd. hh: mm: SS".

>**Observação:** Os valores máximos para propriedades indicados em "dias" são 1 segundo curto do número de dias indicado. Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".

| Propriedade     | Tipo   |Descrição|
|:-------------|:------|:---------|
|Versão|Inteiro|Versão da política. Defina o valor 1. Obrigatório.|
|ApplicationPolicies|Objeto JSON|Conjunto de políticas de aplicativo. Uma política de aplicativo, é uma combinação de uma ApplicationId e uma WebSessionIdleTimeout: <br> <ul><li>**ApplicationId**: valores permitidos:<ul><li> padrão: aplica a política a todos os aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade, mas não têm substituição específica do aplicativo</li><li> c44b4083-3bb0-49c1-b47d-974e53cbdf3c: aplica a política ao portal do Azure</li></ul></li><li>**WebSessionIdleTimeout**: o período de inatividade do usuário após o qual a sessão da Web do usuário é considerada expirada. O valor mínimo é de 5 minutos; o valor máximo é 1 dia.</li></ul> |


## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityBasedTimeoutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
