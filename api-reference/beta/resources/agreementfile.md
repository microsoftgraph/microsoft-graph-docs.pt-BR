---
title: Tipo de recurso agreementFile
description: Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: cd65009ef76c6872b08840157c56255107670bfd
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761874"
---
# <a name="agreementfile-resource-type"></a>Tipo de recurso agreementFile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|Dados que representam os termos de uso do documento PDF. Somente leitura.|
|fileName|String|Nome do arquivo de contrato (por exemplo, TOU.pdf). Somente leitura.|
|id|String|Somente leitura.|
|isDefault|Booliano|Indica se esse é o arquivo de contrato padrão se nenhuma das culturas corresponde à preferência do cliente. Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão. Somente leitura.|
|idioma|Cadeia de caracteres|Cultura do arquivo de contrato no formato languagecode2-country/regioncode2. languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1. country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US). Somente leitura.|
|isMajorVersion|Boolean|Indica se o arquivo de contrato é uma atualização de versão principal. Atualizações de versão principais invalidam as aceitaçãos do contrato no idioma correspondente. |
|createdDateTime|DateTimeOffset|A data que representa quando o arquivo foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é: '2014-01-01T00:00:00Z'.|
|displayName|Cadeia de caracteres|Nome de exibição localizado do arquivo de política de um contrato. O nome de exibição localizado é mostrado aos usuários finais que visualizam o contrato.

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


