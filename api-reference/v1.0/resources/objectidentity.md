---
title: Tipo de recurso objectIdentity
description: Representa uma identidade usada para entrar em uma conta de usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: a7c2e798d08bf0cd2d3a49af017af1d26f054943fbf827cf6f80d0fc45345fd9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235391"
---
# <a name="objectidentity-resource-type"></a>Tipo de recurso objectIdentity

Namespace: microsoft.graph

Representa uma identidade usada para entrar em uma conta de usuário. Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft, que estão vinculados a uma conta de usuário. Isso permite que o usuário entre na conta de usuário com qualquer uma dessas identidades associadas.

A **propriedade** identities do [recurso user](user.md) é um objeto **objectIdentity.**

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|signInType|string| Especifica os tipos de login do usuário em seu diretório, como `emailAddress` , `userName` ou `federated` . Aqui, representa um identificador exclusivo para um usuário de um emissor, que pode estar em qualquer `federated` formato escolhido pelo emissor. A validação adicional é imposta ao **emissorAssignedId** quando o tipo de login é definido como `emailAddress` ou `userName` . Essa propriedade também pode ser definida como qualquer cadeia de caracteres personalizada.|
|emissor|string|Especifica o emissor da identidade, por exemplo `facebook.com` .<br>Para contas locais (onde **signInType** não está ), essa propriedade é o nome de domínio padrão do locatário `federated` B2C local, por exemplo `contoso.onmicrosoft.com` .<br>Para usuários externos de outra organização do Azure AD, este será o domínio da organização federada, por exemplo `contoso.com` .<br><br>Suporta o `$filter`. Limite de 512 caracteres.|
|issuerAssignedId|string|Especifica o identificador exclusivo atribuído ao usuário pelo emissor. A combinação de **emissor e** **emissorAssignedId** deve ser exclusiva dentro da organização. Representa o nome de login do usuário, quando **signInType** é definido como `emailAddress` ou `userName` (também conhecido como contas locais).<br>Quando **signInType** estiver definido como: <ul><li>`emailAddress`, (ou uma cadeia de caracteres personalizada que começa com `emailAddress` como `emailAddress1` ) **emissorAssignedId** deve ser um endereço de email válido</li><li>`userName`, **issuerAssignedId** deve ser uma [parte local válida de um endereço de email](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>Suporta o `$filter`. Limite de 100 caracteres.|

>**Observação:** Ao filtrar na propriedade **identities,**  você deve fornecer emissor e **emissorAssignedId**.

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

