---
title: Tipo de recurso objectIdentity
description: Representa uma identidade usada para entrar em uma conta de usuário.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 93c7fb05945e9924c95031fb8392443acdd0a1ae
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095087"
---
# <a name="objectidentity-resource-type"></a>Tipo de recurso objectIdentity

Namespace: microsoft.graph

Representa uma identidade usada para entrar em uma conta de usuário. Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft, que estão vinculados a uma conta de usuário. Isso permite que o usuário entre na conta de usuário com qualquer uma dessas identidades associadas.

A **propriedade** de identidades do [recurso de](user.md) usuário é um **objeto objectIdentity** .

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|signInType|Cadeia de caracteres| Especifica os tipos de entrada do usuário em seu diretório, como `emailAddress`, `userName`, `federated`ou `userPrincipalName`. `federated` representa um identificador exclusivo para um usuário de um emissor, que pode estar em qualquer formato escolhido pelo emissor. A configuração ou a atualização `userPrincipalName` de uma identidade atualizará o valor da **propriedade userPrincipalName** no objeto de usuário. As validações executadas `userPrincipalName` na propriedade no objeto de usuário, por exemplo, domínios verificados e caracteres aceitáveis, serão executadas ao definir ou atualizar uma `userPrincipalName` identidade. A validação adicional é imposta **em issuerAssignedId** quando o tipo de entrada é definido como `emailAddress` ou `userName`. Essa propriedade também pode ser definida como qualquer cadeia de caracteres personalizada. |
|Emissor|string|Especifica o emissor da identidade, por exemplo `facebook.com`.<br>Para contas locais (onde **signInType** não está `federated`), essa propriedade é o nome de domínio padrão do locatário B2C local, por exemplo `contoso.onmicrosoft.com`.<br>Para usuários externos de Azure AD organização, esse será o domínio da organização federada, por exemplo`contoso.com`.<br><br>Suporta o `$filter`. Limite de 512 caracteres.|
|issuerAssignedId|string|Especifica o identificador exclusivo atribuído ao usuário pelo emissor. A combinação de **issuer** e **issuerAssignedId** deve ser exclusiva dentro da organização. Representa o nome de entrada do usuário, quando **signInType** é definido como `emailAddress` ou `userName` (também conhecido como contas locais).<br>Quando **signInType** é definido como: <ul><li>`emailAddress`, (ou uma cadeia de caracteres personalizada que começa com `emailAddress` like `emailAddress1`), **issuerAssignedId** deve ser um endereço de email válido</li><li>`userName`, **issuerAssignedId** deve ser uma [parte local válida de um endereço de email](https://tools.ietf.org/html/rfc3696#section-3)</li></ul>Suporta o `$filter`. Limite de 100 caracteres.|

### <a name="filtering"></a>Filtragem
Ao filtrar a propriedade **de identidades** para **um issuerAssignedId**, você deve fornecer **o emissor** e **o issuerAssignedId**. Além disso:
- A filtragem de entradas com **um signInType** de `federated` requer um **emissor** válido e **issuerAssignedId**.
- A filtragem de entradas com **um signInType** de `userName` ou `emailAddress` ignora o valor do emissor. Este é o comportamento padrão do produto. 
- Não há suporte para a filtragem de **entradas com um signInType**`userPrincipalName`. Em vez disso, isso pode ser feito filtrando a **propriedade userPrincipalName** no objeto de usuário.

Somente a **filtragem no** emissor tem suporte para os seguintes valores: `google.com`, `facebook.com`, `mail`e `phone`.

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

