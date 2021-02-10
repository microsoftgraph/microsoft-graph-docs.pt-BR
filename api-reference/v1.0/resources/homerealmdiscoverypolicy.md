---
title: Tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56e0d5b0e47c5f3ba5b37e4cbafad2138a2a7e79
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154205"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>Tipo de recurso homeRealmDiscoveryPolicy

Namespace: microsoft.graph

Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para restrições de aceleração automática e autenticação de usuário em domínios federados. Você pode definir **homeRealmDiscoveryPolicy** para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização. Para obter mais cenários e detalhes de política, confira Configurar o comportamento de logon do [Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) para um aplicativo usando uma política de Descoberta de Realm Inicial, bem como entrar no [Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)usando email como uma ID de logon alternativa.

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar homeRealmDiscoveryPolicies](../api/homerealmdiscoverypolicy-list.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Leia as propriedades e as relações dos objetos homeRealmDiscoveryPolicies. |
| [Criar homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Crie um objeto homeRealmDiscoveryPolicy. |
| [Obter homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Ler propriedades e relações de um objeto homeRealmDiscoveryPolicy. |
| [Atualizar homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md) | Nenhum | Atualize um objeto homeRealmDiscoveryPolicy. |
| [Excluir homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-delete.md) | Nenhum | Exclua um objeto homeRealmDiscoveryPolicy. |
| [Lista appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obter a lista de directoryObjects aos qual essa política foi aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo desta política. Somente leitura.|
|definição|Coleção de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Veja abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade. Obrigatório.|
|description|Cadeia de caracteres| Descrição desta política.|
|displayName|Cadeia de caracteres| Nome para exibição desta política. Obrigatório.|
|isOrganizationDefault|Booliano|Se definido como true, ativa essa política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como padrão da organização. Opcional, o valor padrão é false.|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>Propriedades de uma definição de política de descoberta de realm inicial
As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas que** não devem ser inseridas na propriedade de **definição.** Um exemplo é mostrado abaixo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\",
      \"AlternateIdLogin\":{\"Enabled\":true}}}"
  ]
```

| Propriedade     | Tipo   |Descrição| 
|:---------------|:--------|:----------|
|AccelerateToFederatedDomain|Booliano| Definido como `true` para aceleração automática (ignorar descoberta de realm inicial). Se e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade `true` federado (como a ADFS) para entrar. Se `true` houver mais de um domínio verificado no locatário, **PreferredDomain** deverá ser especificado. Opcional.|
|PreferredDomain|Cadeia de caracteres| Especifica um domínio para acelerar a login. Ele poderá ser omitido se o locatário tiver apenas um domínio federado. Se for omitida e houver mais de um domínio federado verificado, essa política não terá efeito. Obrigatório se **AccelerateToFederatedDomain** for `true` .|
|AllowCloudPasswordValidation|Booliano| Definido para permitir que um aplicativo autenti um usuário federado apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade de token do `true` Azure Active Directory. Só funcionará se a Sincronização de Hash de Senha estiver habilitada. Opcional.|
|AlternateIdLogin| Json |De definida como {"Enabled": true} para permitir que o Azure AD entre usando email como uma [ID de logon alternativa.](/azure/active-directory/authentication/howto-authentication-use-email-signin) Só funciona quando **IsOrganizationDefault** está definido como `true` . Opcional.|

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
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
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
  "description": "homeRealmDiscoveryPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
