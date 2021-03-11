---
title: Tipo de recurso objectIdentity
description: Representa uma identidade usada para entrar em uma conta de usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: f646c2c411934b72dfe2ab0ef41d56d363466ae3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722143"
---
# <a name="objectidentity-resource-type"></a>Tipo de recurso objectIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma identidade usada para entrar em uma conta de usuário. Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft, que estão vinculados a uma conta de usuário. Isso permite que o usuário entre na conta de usuário com qualquer uma dessas identidades associadas.

A **propriedade** identities do [recurso user](user.md) é um objeto **objectIdentity.**

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|signInType|cadeia de caracteres| Especifica os tipos de login do usuário em seu diretório, como `emailAddress` , `userName` ou `federated` . Aqui, representa um identificador exclusivo para um usuário de um emissor, que pode estar em qualquer `federated` formato escolhido pelo emissor. A validação adicional é imposta ao **emissorAssignedId** quando o tipo de login é definido como `emailAddress` ou `userName` . Essa propriedade também pode ser definida como qualquer cadeia de caracteres personalizada.|
|emissor|cadeia de caracteres|Especifica o emissor da identidade, por exemplo `facebook.com` .<br>Para contas locais (onde **signInType** não está ), essa propriedade é o nome de domínio padrão do locatário `federated` B2C local, por exemplo `contoso.onmicrosoft.com` .<br>Para usuários externos de outra organização do Azure AD, este será o domínio da organização federada, por exemplo `contoso.com` .<br><br>Oferece suporte para `$filter`. Limite de 512 caracteres.|
|issuerAssignedId|cadeia de caracteres|Especifica o identificador exclusivo atribuído ao usuário pelo emissor. A combinação de **emissor e** **emissorAssignedId** deve ser exclusiva dentro da organização. Representa o nome de login do usuário, quando **signInType** é definido como `emailAddress` ou `userName` (também conhecido como contas locais).<br>Quando **signInType** estiver definido como: <ul><li>`emailAddress`, (ou começa com `emailAddress` o emissor like `emailAddress1` **)AssignedId** deve ser um endereço de email válido</li><li>`userName`, **issuerAssignedId** deve ser uma [parte local válida de um endereço de email](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>Oferece suporte para `$filter`. Limite de 512 caracteres.|

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


