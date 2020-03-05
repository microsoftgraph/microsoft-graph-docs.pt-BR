---
title: tipo de recurso objectidentity
description: Representa uma identidade usada para entrar em uma conta de usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 7eeb5278b2f1d1743177c8d90e496cc719556f94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522523"
---
# <a name="objectidentity-resource-type"></a>tipo de recurso objectidentity

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma identidade usada para entrar em uma conta de usuário. Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft, que estão vinculados a uma conta de usuário. Isso permite que o usuário entre na conta de usuário com qualquer uma dessas identidades associadas.

A propriedade **Identities** do recurso [User](user.md) é um objeto **objectidentity** .

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|signInType|string| Especifica os tipos de entrada do usuário no seu diretório, `emailAddress`como `userName` ou. `federated` Aqui, `federated` representa um identificador exclusivo para um usuário de um emissor, que pode estar em qualquer formato escolhido pelo emissor. A validação adicional é imposta no **issuerAssignedId** quando o tipo de entrada é definido como `emailAddress` ou. `userName` Essa propriedade também pode ser definida como qualquer cadeia de caracteres personalizada.|
|emissor|string|Especifica o emissor da identidade, por exemplo `facebook.com`.<br>Para contas locais (onde **signInType** não `federated`é), essa propriedade é o nome de domínio padrão do locatário do B2C local `contoso.onmicrosoft.com`, por exemplo.<br>Para usuários externos de outra organização do Azure AD, esse será o domínio da organização federada, por exemplo `contoso.com`.<br><br>Suporte `$filter`. limite de caracteres de 512.|
|issuerAssignedId|string|Especifica o identificador exclusivo atribuído ao usuário pelo emissor. A combinação de **Issuer** e **issuerAssignedId** deve ser exclusiva dentro da organização. Representa o nome de entrada do usuário, quando **signInType** é definido como `emailAddress` ou `userName` (também conhecido como contas locais).<br>Quando **signInType** é definido como: <ul><li>`emailAddress`, (ou começa com `emailAddress` like `emailAddress1`) **issuerAssignedId** deve ser um endereço de email válido</li><li>`userName`, **issuerAssignedId** deve ser uma [parte local válida de um endereço de email](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>Suporte `$filter`. limite de caracteres de 512.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectIdentity"
}-->

```json
{
  "signInType": "string",
  "issuer": "string",
  "issuerAssignedId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
