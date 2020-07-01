---
title: tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 143898e33e3e3474bd5caf0d7855ff19a15e4e13
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006965"
---
# <a name="tokenlifetimepolicy-resource-type"></a>tipo de recurso tokenLifetimePolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD). Você pode definir vidas úteis de token para todos os aplicativos em sua organização, para um aplicativo multilocatário (várias organizações) ou para uma entidade de serviço específica em sua organização.  Para obter mais detalhes do cenário, consulte [tempos de vida de token configuráveis no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

>Observação: não há suporte para a configuração dessa política para tokens de atualização e de sessão.

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar tokenLifetimePolicy](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Criar um objeto tokenLifetimePolicy. |
| [Obter tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Ler propriedades e relações de um objeto tokenLifetimePolicy. |
| [Listar tokenLifetimePolicies](../api/tokenlifetimepolicy-list.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Ler propriedades e relações de objetos tokenLifetimePolicies. |
| [Atualizar tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md) | Nenhum | Atualizar um objeto tokenLifetimePolicy. |
| [Excluir tokenLifetimePolicy](../api/tokenlifetimepolicy-delete.md) | Nenhum | Excluir um objeto tokenLifetimePolicy. |
| [Listar se aplica](../api/tokenlifetimepolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obtenha a lista de directoryObjects à qual essa política foi aplicada. |
| [Atribiur tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md) | Nenhum | Atribuir um objeto tokenLifetimePolicy a um objeto [Application](application.md) ou [servicePrincipalName](serviceprincipal.md) . |
| [Lista atribuída tokenLifetimePolicy](../api/application-list-tokenlifetimepolicies.md) | Coleção [tokenLifetimePolicy](tokenlifetimepolicy.md) | Lista os objetos tokenLifetimePolicy que são atribuídos a um objeto [Application](application.md) ou [servicePrincipalName](serviceprincipal.md) . |
| [Remover tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md) | Nenhum | Remover um objeto tokenLifetimePolicy de um objeto [Application](application.md) ou [servicePrincipalName](serviceprincipal.md) . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo da política. Somente leitura.|
|definir|Coleção de cadeias de caracteres| Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política. Veja mais detalhes sobre o esquema JSON para esta propriedade. Obrigatório.|
|description|String| Descrição da política.|
|displayName|Cadeia de caracteres| Nome para exibição dessa política. Obrigatório.|
|isOrganizationDefault|Booliano|Se definido como true, ativa esta política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão. Opcional, o valor padrão é false.|


### <a name="properties-of-a-token-lifetime-policy-definition"></a>Propriedades de uma definição de política de tempo de vida do token
As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token. Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** . Um exemplo é mostrado abaixo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

>Observação: todas as durações de tempo nessas propriedades são especificadas no formato "dd. hh: mm: SS".

>Observação: os valores máximos para propriedades denotadas em "dias" são 1 segundo curto do número de dias indicado. Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".

| Propriedade     | Tipo   |Descrição| Valor mínimo | Valor máximo | Valor padrão|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|Controla por quanto tempo os tokens de acesso e de ID são considerados válidos.|10 minutos|1 dia|1 hora|
|Versão|Número inteiro|Defina o valor 1. Obrigatório.|Nenhum|Nenhum|Nenhum|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appliesTo|Coleção [directoryObject](directoryobject.md)| A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenLifetimePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->