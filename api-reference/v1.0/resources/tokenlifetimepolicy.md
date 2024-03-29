---
title: Tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido por Azure Active Directory.
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f6903abfc318c2b49601ef4aafb2a6d428637504
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143661"
---
# <a name="tokenlifetimepolicy-resource-type"></a>Tipo de recurso tokenLifetimePolicy

Namespace: microsoft.graph



Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD). É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização. 

>**Observação:** Não há suporte para configurar essa política para Tokens de Atualização e Tokens de Sessão.

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar tokenLifetimePolicies](../api/tokenlifetimepolicy-list.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Leia propriedades e relações de objetos tokenLifetimePolicies. |
| [Criar tokenLifetimePolicy](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Crie um objeto tokenLifetimePolicy. |
| [Obter tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | Ler propriedades e relações de um objeto tokenLifetimePolicy. |
| [Atualizar tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md) | Nenhum(a) | Atualize um objeto tokenLifetimePolicy. |
| [Excluir tokenLifetimePolicy](../api/tokenlifetimepolicy-delete.md) | Nenhum(a) | Exclua um objeto tokenLifetimePolicy. |
| [Lista appliesTo](../api/tokenlifetimepolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obter a lista de directoryObjects aos qual essa política foi aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo dessa política. Somente leitura.|
|definition|Coleção String| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade. Obrigatório.|
|description|String| Descrição dessa política.|
|displayName|String| Nome de exibição para esta política. Obrigatório.|
|isOrganizationDefault|Boolean|Se definido como `true` , ativa essa política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização. Opcional, o valor padrão é `false` .|


### <a name="properties-of-a-token-lifetime-policy-definition"></a>Propriedades de uma definição de política de vida útil do token
As propriedades abaixo formam o objeto JSON que representa uma política de vida útil do token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.** Um exemplo é mostrado abaixo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

>**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".

>**Observação:** Os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado. Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".

| Propriedade     | Tipo   |Descrição| Valor Mínimo | Valor Máximo | Valor padrão|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|Controla por quanto tempo os tokens de acesso e ID são considerados válidos.|10 minutos|1 dia|1 hora|
|Versão|Inteiro|Definir o valor de 1. Obrigatório.|Nenhum|Nenhum|Nenhum|

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
