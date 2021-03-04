---
title: Tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 205ac24ace9e0a2a4a4a70af50ef1ac49348d0db
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443031"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>Tipo de recurso homeRealmDiscoveryPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para restrições de aceleração automática e autenticação do usuário em domínios federados. Você pode definir homeRealmDiscoveryPolicy para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização.  Para obter mais detalhes de cenário e política, consulte [Configure Azure AD sign in](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) behavior for an application by using a Home Realm Discovery policy, well as [Sign-in to Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)using email as an alternate login ID .

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Crie um objeto homeRealmDiscoveryPolicy. |
| [Obter homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Leia propriedades e relações de um objeto homeRealmDiscoveryPolicy. |
| [Listar homeRealmDiscoveryPolicies](../api/homerealmdiscoverypolicy-list.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Ler propriedades e relações de objetos homeRealmDiscoveryPolicies. |
| [Atualizar homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md) | Nenhum(a) | Atualize um objeto homeRealmDiscoveryPolicy. |
| [Excluir homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-delete.md) | Nenhum(a) | Exclua um objeto homeRealmDiscoveryPolicy. |
| [Lista appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obter a lista de directoryObjects aos qual essa política foi aplicada. |
| [Atribuir homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md) | Nenhum(a) | Atribua um objeto homeRealmDiscoveryPolicy a um [objeto servicePrincipal.](serviceprincipal.md) |
| [Listar homeRealmDiscoveryPolicy atribuída](../api/serviceprincipal-list-homerealmdiscoverypolicies.md) | Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Listar os objetos homeRealmDiscoveryPolicy atribuídos a um [objeto servicePrincipal.](serviceprincipal.md) |
| [Remover homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md) | Nenhum(a) | Remova um objeto homeRealmDiscoveryPolicy de [um objeto servicePrincipal.](serviceprincipal.md) |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo dessa política. Somente leitura.|
|definition|Coleção de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade. Obrigatório.|
|description|String| Descrição dessa política.|
|displayName|String| Nome de exibição para esta política. Obrigatório.|
|isOrganizationDefault|Booliano|Se definido como true, ativa essa política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização. Opcional, o valor padrão é false.|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>Propriedades de uma definição de política de descoberta de domínio inicial
As propriedades abaixo formam o objeto JSON que representa uma política de vida útil do token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.** Um exemplo é mostrado abaixo no formato JSON:

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
|AccelerateToFederatedDomain|Booliano| Definir como `true` para aceleração automática (ignorar descoberta de domínio inicial). Se e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade `true` federado (como ADFS) para entrar. Se `true` e houver mais de um domínio verificado no locatário, **PreferredDomain** deve ser especificado. Opcional.|
|PreferredDomain|String| Especifica um domínio para acelerar a login. Ele pode ser omitido se o locatário tiver apenas um domínio federado. Se for omitido e houver mais de um domínio federado verificado, essa política não terá efeito. Obrigatório se **AccelerateToFederatedDomain** for `true` .|
|AllowCloudPasswordValidation|Booliano| De acordo com a opção de permitir que um aplicativo autenture um usuário federado apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade do token do `true` Azure Active Directory. Só funciona se a Sincronização de Hash de Senha estiver habilitada. Opcional.|
|AlternateIdLogin| Json |De acordo com {"Enabled": true} para permitir a logon do Azure AD usando o email como uma [ID de logon alternativa.](/azure/active-directory/authentication/howto-authentication-use-email-signin) Só funciona quando **IsOrganizationDefault** é definido como `true` . Opcional.|

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
