---
title: Tipo de recurso identityProviderBase
description: Representa provedores de identidade em um locatário do Azure Active Directory e um locatário do B2C do Azure AD
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 1a3d26697c26b803bcbac9141d7ff011575f91f7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491072"
---
# <a name="identityproviderbase-resource-type"></a>Tipo de recurso identityProviderBase
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa provedores de identidade com [Identidades externas](/azure/active-directory/external-identities/) para locatário do Azure Active Directory e um locatário do Azure AD B2C.

Para cenários do Azure AD B2B em um diretório do Azure AD, o provedor de identidade pode ser um [provedor de identidade social](../resources/socialidentityprovider.md) ou um [provedor de identidade interno](../resources/builtinidentityprovider.md), que herdará do tipo de recurso base do provedor de identidade.

Configurar um provedor de identidade em seu diretório do Azure AD permite novos cenários de convidado do Azure AD B2B. Por exemplo, uma organização possui recursos no Microsoft 365 que precisam ser compartilhados com um usuário do Gmail. O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.

Em um diretório Azure AD B2C, o tipo de provedor de identidade podem ser [Provedores de identidade social](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [appleIdentityProvider](../resources/appleidentityprovider.md), que herdará do tipo de recurso identityProviderBase. 

Configurar um provedor de identidade no diretório do Azure AD B2C permite que os usuários se inscrevam e entrem usando uma conta social ou um provedor com suporte OpenID Connect personalizado em um aplicativo. Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook ou o seu próprio provedor de identidade personalizado que esteja em conformidade com o protocolo OIDC.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identityproviderbase-list.md)|Coleção identityProviderBase|Recupere todos os provedores de identidade configurados em um locatário.|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-list-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recupere todos os tipos de provedor de identidade disponíveis no locatário.|

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
    "displayName": "String",
}
```
