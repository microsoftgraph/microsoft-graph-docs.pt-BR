---
title: tipo de recurso objectidentity
description: Representa uma identidade usada para entrar em uma conta de usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: d14de40c6be6564dcb53436aa6ea1400914bca15
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905208"
---
# <a name="objectidentity-resource-type"></a>tipo de recurso objectidentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma identidade usada para entrar em uma conta de usuário. Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft, que estão vinculados a uma conta de usuário. Isso permite que o usuário entre na conta de usuário com qualquer uma dessas identidades associadas.

A propriedade **Identities** do recurso [User](user.md) é um objeto **objectidentity** .

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|signInType|string| Especifica os tipos de entrada do usuário no seu diretório, como `emailAddress` `userName` ou `federated` . Aqui, `federated` representa um identificador exclusivo para um usuário de um emissor, que pode estar em qualquer formato escolhido pelo emissor. A validação adicional é imposta no **issuerAssignedId** quando o tipo de entrada é definido como `emailAddress` ou `userName` . Essa propriedade também pode ser definida como qualquer cadeia de caracteres personalizada.|
|emissor|string|Especifica o emissor da identidade, por exemplo `facebook.com` .<br>Para contas locais (onde **signInType** não é `federated` ), essa propriedade é o nome de domínio padrão do locatário do B2C local, por exemplo `contoso.onmicrosoft.com` .<br>Para usuários externos de outra organização do Azure AD, esse será o domínio da organização federada, por exemplo `contoso.com` .<br><br>Oferece suporte para `$filter`. limite de caracteres de 512.|
|issuerAssignedId|string|Especifica o identificador exclusivo atribuído ao usuário pelo emissor. A combinação de **Issuer** e **issuerAssignedId** deve ser exclusiva dentro da organização. Representa o nome de entrada do usuário, quando **signInType** é definido como `emailAddress` ou `userName` (também conhecido como contas locais).<br>Quando **signInType** é definido como: <ul><li>`emailAddress`, (ou começa com `emailAddress` like `emailAddress1` ) **issuerAssignedId** deve ser um endereço de email válido</li><li>`userName`, **issuerAssignedId** deve ser uma [parte local válida de um endereço de email](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>Oferece suporte para `$filter`. limite de caracteres de 512.|

>**Observação:** Ao filtrar na propriedade **Identities** , você deve fornecer o **emissor** e o **issuerAssignedId**.

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


