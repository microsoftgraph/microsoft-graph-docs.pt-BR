---
title: Tipo de recurso appleManagedIdentityProvider
description: Representa o provedor de identidade da Apple em um locatário do Azure AD B2C.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ce307ea651515482c6c82baa91c8fe4dcd598219
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891240"
---
# <a name="applemanagedidentityprovider-resource-type"></a>Tipo de recurso appleManagedIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o provedor de identidade da Apple em um locatário do Azure AD B2C.

Você pode configurar a Apple como um provedor de identidade social para um locatário do B2C do Azure AD Com base nas informações fornecidas pela Apple, a API irá gerar um segredo do cliente. A Apple precisa que o segredo seja renovado a cada seis meses. Você terá que girar o segredo manualmente.

Herdado de [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|Coleção [identityProviderBase](../resources/identityproviderbase.md) |Recupere todos os provedores de identidade configurados em um locatário, incluindo os provedores de identidade da Apple. Não há como recuperar apenas os provedores de identidade da Apple em um locatário.|
|[Criar](../api/identitycontainer-post-identityproviders.md)|[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |Criae uma nova configuração de provedor de identidade Apple.|
|[Get](../api/identityproviderbase-get.md) |[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |Recuperar propriedades da configuração do provedor de identidade Apple.|
|[Atualizar](../api/identityproviderbase-update.md)|Nenhum(a)|Atualizar a configuração do provedor de identidade Apple.|
|[Delete](../api/identityproviderbase-delete.md)|Nenhum|Excluir a configuração do provedor de identidade Apple.|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recuperar todos os tipos de provedores de identidade disponíveis no locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|certificateData|Cadeia de caracteres|Os dados do certificado, que é uma longa cadeia de caracteres de texto do certificado. Pode ser nulo.|
|developerId|Cadeia de caracteres|O identificador de desenvolvedor da Apple. Obrigatório.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Herdado de [identityProviderBase](../resources/identityproviderbase.md). Somente leitura.|
|keyId|Cadeia de caracteres|O identificador de chave da Apple. Obrigatório.|
|serviceId|Cadeia de caracteres|O identificador de serviço da Apple. Obrigatório.|

Recupere o **developerId**, **serviceId**, **keyId**, e os **certificateData** do portal do desenvolvedor da Apple. Para obter mais informações, siga o guia para [ criar um aplicativo de ID da Apple](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```json
{
    "id": "String",
    "displayName": "String",
    "developerId": "String",
    "serviceId": "String",
    "keyId": "String",
    "certificateData": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "appleIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
