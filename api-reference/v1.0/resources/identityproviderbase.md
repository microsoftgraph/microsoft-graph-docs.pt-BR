---
title: Tipo de recurso identityProviderBase
description: Representa provedores de identidade em um locatário do Azure Active Directory e um locatário do B2C do Azure AD
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 661c9ca5f1a76af52112d22671d02bd2c801b79f
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890168"
---
# <a name="identityproviderbase-resource-type"></a>Tipo de recurso identityProviderBase
Namespace: microsoft.graph

Representa provedores de identidade com [Identidades Externas](/azure/active-directory/external-identities/) para locatários do Azure Active Directory (Azure Active Directory) e do Azure Active Directory B2C.

Para cenários do Azure Active Directory B2B em um diretório do Azure Active Directory, o provedor de identidade pode ser um [socialIdentityProvider](../resources/socialidentityprovider.md) ou [builtinIdentityProvider](../resources/builtinidentityprovider.md), ambos herdados do tipo de recurso identityProviderBase.

Configurar um provedor de identidade em seu diretório do Azure AD permite novos cenários de convidado do Azure AD B2B. Por exemplo, uma organização possui recursos no Microsoft 365 que precisam ser compartilhados com um usuário do Gmail. O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.

Em um diretório B2C do Azure AD, o tipo de provedor de identidade pode ser um [socialIdentityProvider](../resources/socialidentityprovider.md) ou um [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md), todos herdados do tipo de recurso identityProviderBase.

Configurar um provedor de identidade no diretório do Azure AD B2C permite que os usuários se inscrevam e entrem usando uma conta social ou um provedor com suporte OpenID Connect personalizado em um aplicativo. Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook ou o seu próprio provedor de identidade personalizado que esteja em conformidade com o protocolo OIDC.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|Coleção [identityProviderBase](../resources/identityproviderbase.md) |Recupere todos os provedores de identidade configurados em um locatário.|
|[Criar](../api/identitycontainer-post-identityproviders.md)| [socialidentityprovider](../resources/socialidentityprovider.md) ou  [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |Crie um novo objeto de um dos seguintes tipos de objeto: <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md) (Azure Active Directory ou Azure Active Directory B2C) <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) (Azure Active Directory B2C) </li></ul>|
|[Get](../api/identityproviderbase-get.md) |[socialidentityprovider](../resources/socialidentityprovider.md), [builtInIdentityProvider](../resources/builtinidentityprovider.md) ou  [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)| Recupere as propriedades de um dos seguintes tipos de objeto: <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md) (Azure Active Directory ou Azure Active Directory B2C) <li> [builtInIdentityProvider](../resources/builtinidentityprovider.md) (Azure Active Directory ou Azure Active Directory B2C) <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) (Azure Active Directory B2C) </li></ul>|
|[Atualizar](../api/identityproviderbase-update.md)|Nenhum(a)|Atualize um dos seguintes tipos de objeto: <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md) (Azure Active Directory ou Azure Active Directory B2C) <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) (Azure Active Directory B2C) </li></ul>|
|[Delete](../api/identityproviderbase-delete.md)|Nenhum|Exclua um dos seguintes tipos de objeto: <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md) (Azure Active Directory ou Azure Active Directory B2C) <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) (Azure Active Directory B2C) (Azure Active Directory B2C)|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recuperar todos os tipos de provedores de identidade disponíveis no locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O identificador do provedor de identidade.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String"
}
```
