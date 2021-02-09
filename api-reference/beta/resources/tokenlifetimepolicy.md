---
title: Tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bcfe06a8a42db4b0cfd5c8dab8da2b753e195f2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155500"
---
# <a name="tokenlifetimepolicy-resource-type"></a>Tipo de recurso tokenLifetimePolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD). É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização.  Para obter mais detalhes do cenário, [consulte Tempo de vida de token configurável no Azure Active Directory.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

>Observação: a configuração dessa política para Tokens de Atualização e Tokens de Sessão não é suportada.

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar tokenLifetimePolicy](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Crie um objeto tokenLifetimePolicy. |
| [Obter tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Ler propriedades e relações de um objeto tokenLifetimePolicy. |
| [Listar tokenLifetimePolicies](../api/tokenlifetimepolicy-list.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Leia as propriedades e os relacionamentos dos objetos tokenLifetimePolicies. |
| [Atualizar tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md) | Nenhum(a) | Atualize um objeto tokenLifetimePolicy. |
| [Excluir tokenLifetimePolicy](../api/tokenlifetimepolicy-delete.md) | Nenhum(a) | Exclua um objeto tokenLifetimePolicy. |
| [Lista appliesTo](../api/tokenlifetimepolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obter a lista de directoryObjects aos qual essa política foi aplicada. |
| [Atribiur tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md) | Nenhum(a) | Atribua um objeto tokenLifetimePolicy a [um aplicativo ou](application.md) objeto [servicePrincipal.](serviceprincipal.md) |
| [Listar tokenLifetimePolicy atribuído](../api/application-list-tokenlifetimepolicies.md) | Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md) | Listar os objetos tokenLifetimePolicy atribuídos a um [aplicativo ou](application.md) [objeto servicePrincipal.](serviceprincipal.md) |
| [Remover tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md) | Nenhum(a) | Remova um objeto tokenLifetimePolicy de um [aplicativo ou](application.md) [objeto servicePrincipal.](serviceprincipal.md) |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo desta política. Somente leitura.|
|definição|Coleção de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Veja abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade. Obrigatório.|
|description|String| Descrição desta política.|
|displayName|String| Nome para exibição desta política. Obrigatório.|
|isOrganizationDefault|Boolean|Se definido como true, ativa essa política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como padrão da organização. Opcional, o valor padrão é false.|


### <a name="properties-of-a-token-lifetime-policy-definition"></a>Propriedades de uma definição de política de tempo de vida do token
As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres** com aspas que não devem ser inseridas na propriedade de **definição.** Um exemplo é mostrado abaixo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

>Observação: todas as durações nessas propriedades são especificadas no formato "dd.hh:mm:ss".

>Observação: os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado. Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".

| Propriedade     | Tipo   |Descrição| Valor Mínimo | Valor Máximo | Valor padrão|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|Controla por quanto tempo os tokens de acesso e de ID são considerados válidos.|10 minutos|1 dia|1 hora|
|Versão|Inteiro|Valor definido de 1. Obrigatório.|Nenhum|Nenhum|Nenhum|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appliesTo|Coleção [directoryObject](directoryobject.md)| A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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