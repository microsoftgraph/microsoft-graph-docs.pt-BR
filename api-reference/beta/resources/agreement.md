---
title: tipo de recurso de contrato
description: Representa os termos personalizável de um locatário contrato de uso que é criado e gerenciado com o Azure Active Directory (AD Azure). Você pode usar os métodos a seguir para criar e gerenciar o recurso do Windows Azure Active Directory termos de uso de acordo com o seu cenário.
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513848"
---
# <a name="agreement-resource-type"></a>tipo de recurso de contrato

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os termos personalizável de um locatário contrato de uso que é criado e gerenciado com o Azure Active Directory (AD Azure). Você pode usar os métodos a seguir para criar e gerenciar o [Azure Active Directory termos de uso de recurso](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) de acordo com seu cenário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar contratos](../api/agreement-post-agreements.md) | [contrato](agreement.md) | Crie um novo contrato pelo lançamento à coleção contrato. |
| [Contratos de lista](../api/agreement-list.md) | coleção de [contrato](agreement.md) | Obtenha uma coleção de objetos do contrato. |
| [Obter contrato](../api/agreement-get.md) | [contrato](agreement.md) | Leia as propriedades e os relacionamentos de um objeto de contrato. |
| [Atualizar contrato](../api/agreement-update.md) | [contrato](agreement.md) | Atualize um objeto de contrato. |
| [Excluir contrato](../api/agreement-delete.md) | Nenhum | Exclua um objeto de contrato. |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String|Nome para exibição do contrato.|
|id|String| Somente leitura.|
|isViewingBeforeAcceptanceRequired|Booliano|Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|arquivos|coleção [agreementFile](agreementfile.md)|Somente leitura. PDFs vinculada a este contrato.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
