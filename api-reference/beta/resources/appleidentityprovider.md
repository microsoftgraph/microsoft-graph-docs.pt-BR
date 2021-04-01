---
title: Tipo de recurso appleManagedIdentityProvider
description: Representa o provedor de identidade apple em um locatário do B2C do Azure AD
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ee02900b6d41695d49d7c5ee38d834c676f69603
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491065"
---
# <a name="applemanagedidentityprovider-resource-type"></a>Tipo de recurso appleManagedIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode configurar a Apple como um provedor de identidade social para um locatário do B2C do Azure AD Com base nas informações fornecidas pela Apple, a API irá gerar um segredo do cliente. A Apple precisa que o segredo seja renovado a cada seis meses. Você terá que girar o segredo manualmente.

Este tipo herdará de [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identityproviderbase-list.md)|Coleção identityProviderBase|Recupere todos os provedores de identidade configurados em um locatário, incluindo os provedores de identidade Apple.|
|[Create](../api/identityproviderbase-post-identityproviders.md)|appleManagedIdentityProvider |Criae uma nova configuração de provedor de identidade Apple.|
|[Get](../api/identityproviderbase-get.md) |appleManagedIdentityProvider |Recuperar propriedades da configuração do provedor de identidade Apple.|
|[Atualizar](../api/identityproviderbase-update.md)|Nenhum(a)|Atualizar a configuração do provedor de identidade Apple.|
|[Delete](../api/identityproviderbase-delete.md)|Nenhum|Excluir a configuração do provedor de identidade Apple.|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-list-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recuperar todos os tipos de provedor de identidade disponíveis no locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|developerId|Cadeia de caracteres|O Identificador de desenvolvedor da Apple. Obrigatório.|
|serviceId|Cadeia de caracteres|O identificador de serviço da Apple. Obrigatório.|
|keyId|Cadeia de caracteres|O identificador de chave da Apple. Obrigatório.|
|certificateData|Cadeia de caracteres|Os dados do certificado, que são uma longa sequência de texto do certificado, podem ser nulos.|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Herdado de [identityProviderBase](../resources/identityproviderbase.md). Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|

Você pode encontrar o developerId, serviceId, keyId e o certificateData no portal do desenvolvedor da Apple. Para obter mais detalhes, você pode seguir o guia para [criar um aplicativo Apple ID](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)

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
