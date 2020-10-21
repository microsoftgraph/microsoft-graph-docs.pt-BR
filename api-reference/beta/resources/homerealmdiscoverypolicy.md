---
title: tipo de recurso homeRealmDiscoveryPolicy
description: Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 694309327fe122a0053039d527321f0f4afb0751
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635156"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>tipo de recurso homeRealmDiscoveryPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política para controlar o comportamento de autenticação do Azure Active Directory para usuários federados, em particular para as restrições de aceleração automática e autenticação de usuário em domínios federados. Você pode definir homeRealmDiscoveryPolicy para todas as entidades de serviço em sua organização ou para entidades de serviço específicas em sua organização.  Para obter mais detalhes de cenário e política, consulte [Configurar o comportamento de entrada do Azure ad para um aplicativo usando uma política de descoberta de realm inicial](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) , bem como [entrar no Azure Active Directory usando email como uma ID de logon alternativa](/azure/active-directory/authentication/howto-authentication-use-email-signin).

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Criar um objeto homeRealmDiscoveryPolicy. |
| [Obter homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Ler propriedades e relações de um objeto homeRealmDiscoveryPolicy. |
| [Listar homeRealmDiscoveryPolicies](../api/homerealmdiscoverypolicy-list.md) | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Ler propriedades e relações de objetos homeRealmDiscoveryPolicies. |
| [Atualizar homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md) | Nenhum | Atualizar um objeto homeRealmDiscoveryPolicy. |
| [Excluir homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-delete.md) | Nenhum | Excluir um objeto homeRealmDiscoveryPolicy. |
| [Listar se aplica](../api/homerealmdiscoverypolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obtenha a lista de directoryObjects à qual essa política foi aplicada. |
| [Atribuir homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md) | Nenhum | Atribuir um objeto homeRealmDiscoveryPolicy a um objeto [servicePrincipalName](serviceprincipal.md) . |
| [Lista atribuída homeRealmDiscoveryPolicy](../api/serviceprincipal-list-homerealmdiscoverypolicies.md) | Conjunto [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Lista os objetos homeRealmDiscoveryPolicy que são atribuídos a um objeto [servicePrincipalName](serviceprincipal.md) . |
| [Remover homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md) | Nenhum | Remover um objeto homeRealmDiscoveryPolicy de um objeto [servicePrincipalName](serviceprincipal.md) . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo da política. Somente leitura.|
|definir|Conjunto de cadeias de caracteres| Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política. Veja mais detalhes sobre o esquema JSON para esta propriedade. Obrigatório.|
|description|String| Descrição da política.|
|displayName|String| Nome para exibição dessa política. Obrigatório.|
|isOrganizationDefault|Booleano|Se definido como true, ativa esta política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão. Opcional, o valor padrão é false.|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>Propriedades de uma definição de política de descoberta de realm inicial
As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token. Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** . Um exemplo é mostrado abaixo no formato JSON:

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
|AccelerateToFederatedDomain|Booleano| Defina como `true` para aceleração automática (bypass da descoberta de realm inicial). Se `true` e houver apenas um domínio verificado e federado no locatário, os usuários serão levados diretamente para o provedor de identidade federada (como ADFS) para entrar. Se `true` houver mais de um domínio verificado no locatário, **PreferredDomain** deverá ser especificado. Opcional.|
|PreferredDomain|String| Especifica um domínio para o qual acelerar o logon. Ele pode ser omitido se o locatário tiver apenas um domínio federado. Se for omitido e houver mais de um domínio federado verificado, essa política não terá efeito. Obrigatório se **AccelerateToFederatedDomain** for `true` .|
|AllowCloudPasswordValidation|Booleano| Defina como `true` para permitir que um aplicativo autentique um usuário federado, apresentando credenciais de nome de usuário/senha diretamente para o ponto de extremidade de token do Azure Active Directory. Funcionará somente se a sincronização de hash de senha estiver habilitada. Opcional.|
|AlternateIdLogin| Json |Defina como {"Enabled": true} para permitir a entrada do Azure AD usando email como [uma ID de logon alternativa](https://docs.microsoft.com/azure/active-directory/authentication/howto-authentication-use-email-signin). Só funciona quando **IsOrganizationDefault** está definido como `true` . Opcional.|

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
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
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
  "description": "homeRealmDiscoveryPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
