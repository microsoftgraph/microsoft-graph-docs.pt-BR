---
title: Tipo de recurso identityProviderBase
description: Representa provedores de identidade em um locatário do Azure Active Directory e um locatário do B2C do Azure AD
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: aacf2b128e8cf60f445fb59d93e6be8d84b8deb0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032381"
---
# <a name="identityproviderbase-resource-type"></a>Tipo de recurso identityProviderBase
Namespace: microsoft.graph

Representa provedores de identidade com [Identidades Externas](/azure/active-directory/external-identities/) para locatários do Azure Active Directory (Azure AD) e do Azure AD B2C. É um tipo abstrato herdado pelo [socialIdentityProvider](../resources/socialidentityprovider.md) e [builtinIdentityProvider](../resources/builtinidentityprovider.md).

Para cenários do Microsoft Azure AD B2B , o provedor de identidade é um [socialIdentityProvider](../resources/socialidentityprovider.md) ou um [builtinIdentityProvider](../resources/builtinidentityprovider.md). A configuração de um provedor de identidade no seu locatário do Microsoft Azure Active Directory permite novos cenários de convidados do Microsoft Azure AD B2B. Por exemplo, uma organização com recursos no Microsoft 365 pode compartilhá-los com um usuário do Gmail. O usuário do Gmail usará as credenciais da conta do Google para autenticar e acessar os documentos.

Em um diretório do Azure AD B2C, o tipo de provedor de identidade é um [socialIdentityProvider](../resources/socialidentityprovider.md). Configurar um provedor de identidade no seu diretório do Azure AD B2C permite que os usuários se inscrevam e entrem usando uma conta social em um aplicativo. Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|Coleção [identityProviderBase](../resources/identityproviderbase.md) |Recupere todos os provedores de identidade configurados em um locatário.|
|[Criar](../api/identitycontainer-post-identityproviders.md)|[socialIdentityProvider](../resources/socialidentityprovider.md)|Criar um novo [socialIdentityProvider](../resources/socialidentityprovider.md) (Azure AD ou Azure AD B2C).|
|[Obter](../api/identityproviderbase-get.md) |[socialIdentityProvider](../resources/socialidentityprovider.md) ou [builtinIdentityProvider](../resources/builtinidentityprovider.md)|Recupere as propriedades de um [socialIdentityProvider](../resources/socialidentityprovider.md) (Azure AD or Azure AD B2C) ou um [builtinIdentityProvider](../resources/builtinidentityprovider.md) (Azure AD).|
|[Atualizar](../api/identityproviderbase-update.md)|Nenhum(a)|Atualize um [socialIdentityProvider](../resources/socialidentityprovider.md) (Azure AD ou Azure AD B2C).|
|[Delete](../api/identityproviderbase-delete.md)|Nenhum|Excluir um [socialIdentityProvider](../resources/socialidentityprovider.md) (Azure AD ou Azure AD B2C).|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recupere todos os tipos de provedores de identidade com suporte.|

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
