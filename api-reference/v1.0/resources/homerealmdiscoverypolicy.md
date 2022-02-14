---
title: Tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o Azure Active Directory de autenticação para usuários federados.
ms.localizationpriority: medium
author: hpsin
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: dec8466594981602cf6d933e26a5b2b0214ae011
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804735"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>Tipo de recurso homeRealmDiscoveryPolicy

Namespace: microsoft.graph

Representa uma política para controlar Azure Active Directory de autenticação para usuários federados, em particular para restrições de aceleração automática e autenticação do usuário em domínios federados. Você pode definir **homeRealmDiscoveryPolicy** para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização. Para obter mais detalhes de cenário e política, consulte [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal), well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar homeRealmDiscoveryPolicies](../api/homerealmdiscoverypolicy-list.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Ler propriedades e relações de objetos homeRealmDiscoveryPolicies. |
| [Criar homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Crie um objeto homeRealmDiscoveryPolicy. |
| [Obter homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Leia propriedades e relações de um objeto homeRealmDiscoveryPolicy. |
| [Atualizar homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md) | Nenhum | Atualize um objeto homeRealmDiscoveryPolicy. |
| [Excluir homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-delete.md) | Nenhum | Exclua um objeto homeRealmDiscoveryPolicy. |
| [Lista appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obter a lista de directoryObjects aos qual essa política foi aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo dessa política. Somente leitura.|
|definition|String collection| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Consulte [Propriedades de uma definição de política de](#properties-of-a-home-realm-discovery-policy-definition) descoberta de domínio inicial para obter mais detalhes sobre o esquema JSON para essa propriedade. Obrigatório.|
|description|Cadeia de caracteres| Descrição dessa política.|
|displayName|Cadeia de caracteres| Nome de exibição para esta política. Obrigatório.|
|isOrganizationDefault|Boolean|Se definido como `true`, ativa essa política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização. Opcional, o valor padrão é `false`.|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>Propriedades de uma definição de política de descoberta de domínio inicial
As propriedades abaixo formam o objeto JSON que representa uma política de vida útil do token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na **propriedade definition** . Um exemplo é mostrado abaixo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{
        \"HomeRealmDiscoveryPolicy\": {
          \"AccelerateToFederatedDomain\":true,
          \"AllowCloudPasswordValidation\": false,
          \"PreferredDomain\":\"federated.example.edu\",
          \"AlternateIdLogin\":{
            \"Enabled\":true
          }
        }
      }"
  ]
```

| Propriedade     | Tipo   |Descrição| 
|:---------------|:--------|:----------|
|AccelerateToFederatedDomain|Boolean| Definir como para `true` aceleração automática (ignorar descoberta de domínio inicial). Se `true` e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade federado (como ADFS) para entrar. Se `true` e houver mais de um domínio verificado no locatário, **PreferredDomain** deve ser especificado. Opcional.|
|AllowCloudPasswordValidation|Boolean| De definida para `true` permitir que um aplicativo autenture um usuário federado apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade Azure Active Directory token. Só funciona se a Sincronização de Hash de Senha estiver habilitada. Opcional.|
|AlternateIdLogin| Json |De definida para `{\"Enabled\": true}` permitir a logon do Azure AD usando email como [uma ID de logon alternativa](/azure/active-directory/authentication/howto-authentication-use-email-signin). Só funciona quando **IsOrganizationDefault** é definido como `true`. Opcional.|
|PreferredDomain|Cadeia de caracteres| Especifica um domínio para acelerar a login. Ele pode ser omitido se o locatário tiver apenas um domínio federado. Se for omitido e houver mais de um domínio federado verificado, essa política não terá efeito. Obrigatório se **AccelerateToFederatedDomain** for `true`.|

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
