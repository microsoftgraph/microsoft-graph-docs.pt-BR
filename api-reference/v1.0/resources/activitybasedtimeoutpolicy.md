---
title: Tipo de recurso activityBasedTimeoutPolicy
description: Representa uma política que pode controlar o tempo de inativo para sessões da Web para aplicativos que suportam a funcionalidade de tempo de tempo de atividade baseada em atividade.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e5812642961dfd1481cba110052fa767700b0ad0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159000"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a>Tipo de recurso activityBasedTimeoutPolicy

Namespace: microsoft.graph

Representa uma política que pode controlar o tempo de inativo para sessões da Web para aplicativos que suportam a funcionalidade de tempo de tempo de atividade baseada em atividade. Os aplicativos impõem a inscrição automática após um período de inatividade. Esse tipo de política só pode ser aplicado no nível da organização (definindo a **propriedade isOrganizationDefault** como `true` ).

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar activityBasedTimeoutPolicies](../api/activitybasedtimeoutpolicy-list.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Leia as propriedades e os relacionamentos dos objetos activityBasedTimeoutPolicy. |
| [Criar activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Criar um objeto activityBasedTimeoutPolicy. |
| [Obter activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-get.md) | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) | Ler propriedades e relações de um objeto activityBasedTimeoutPolicy. |
| [Atualizar activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-update.md) | Nenhum | Atualize um objeto activityBasedTimeoutPolicy. |
| [Excluir activityBasedTimeoutPolicy](../api/activitybasedtimeoutpolicy-delete.md) | Nenhum | Exclua um objeto activityBasedTimeoutPolicy. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo desta política. Somente leitura.|
|definição|Coleção de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Veja abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade. Obrigatório.|
|description|Cadeia de caracteres| Descrição desta política.|
|displayName|Cadeia de caracteres| Nome para exibição desta política. Obrigatório.|
|isOrganizationDefault|Booliano|Se definido como true, ativa essa política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como padrão da organização. Opcional, o valor padrão é false.|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a>Propriedades de uma definição de política de tempo de vida baseada em atividade
As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida baseada em atividade. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas que** não devem ser inseridas na propriedade de **definição.** Um exemplo é mostrado abaixo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

>**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".

>**Observação:** Os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado. Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".

| Propriedade     | Tipo   |Descrição|
|:-------------|:------|:---------|
|Versão|Inteiro|Versão da política. Valor definido de 1. Obrigatório.|
|ApplicationPolicies|Objeto JSON|Coleção de política de aplicativo. Uma política de aplicativo é uma combinação de ApplicationId e WebSessionIdleTimeout: <br> <ul><li>**ApplicationId**: valores permitidos:<ul><li> padrão: aplica a política a todos os aplicativos que suportam a funcionalidade de tempoout baseada em atividade, mas não têm substituição específica do aplicativo</li><li> c44b4083-3bb0-49c1-b47d-974e53cbdf3c: aplica a política ao Portal do Azure</li></ul></li><li>**WebSessionIdleTimeout**: o período de inatividade do usuário após o qual a sessão da Web do usuário é considerada expirada. O valor mínimo é 5 minutos; o valor máximo é de 1 dia.</li></ul> |


## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
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

