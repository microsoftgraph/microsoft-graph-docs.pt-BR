---
title: tipo de recurso de contrato
description: Representa os termos personalizável de um locatário contrato de uso que é criado e gerenciado com o Azure Active Directory (AD Azure). Você pode usar os métodos a seguir para criar e gerenciar o recurso do Windows Azure Active Directory termos de uso de acordo com o seu cenário.
ms.openlocfilehash: 2e5c9087cd809f9c067150654d420fda533ca61b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035469"
---
# <a name="agreement-resource-type"></a>tipo de recurso de contrato

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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

## <a name="relationships"></a>Relações
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
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
