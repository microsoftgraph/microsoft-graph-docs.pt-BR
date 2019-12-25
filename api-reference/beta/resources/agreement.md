---
title: tipo de recurso de contrato
description: Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o recurso termos de uso do Azure Active Directory de acordo com seu cenário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d698aa85f38061ce22d63f37ea3deca3635ba219
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870950"
---
# <a name="agreement-resource-type"></a>tipo de recurso de contrato

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o [recurso termos de uso do Azure Active Directory de](/azure/active-directory/active-directory-tou) acordo com seu cenário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar contratos](../api/agreement-post-agreements.md) | [contrato](agreement.md) | Crie um novo contrato postando na coleção de contratos. |
| [Listar contratos](../api/agreement-list.md) | coleção de [contratos](agreement.md) | Obtenha uma coleção de objetos de contrato. |
| [Obter contrato](../api/agreement-get.md) | [contrato](agreement.md) | Leia as propriedades e as relações de um objeto de contrato. |
| [Atualizar contrato](../api/agreement-update.md) | [contrato](agreement.md) | Atualize um objeto de contrato. |
| [Excluir contrato](../api/agreement-delete.md) | Nenhum | Exclua um objeto de contrato. |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Nome para exibição do contrato.|
|id|String| Somente leitura.|
|isViewingBeforeAcceptanceRequired|Booliano|Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|arquivos|coleção [agreementfile](agreementfile.md)|Somente leitura. PDFs vinculados a este contrato.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
