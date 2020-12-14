---
title: tipo de recurso contratofile
description: Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 12c45876558a162b910120e62c6997c251f391e1
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664020"
---
# <a name="agreementfile-resource-type"></a>tipo de recurso contratofile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).

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
|fileData|[agreementFileData](agreementfiledata.md)|Dados que representam o documento PDF termos de uso. Somente leitura.|
|fileName|String|Nome do arquivo de contrato (por exemplo, TOU.pdf). Somente leitura.|
|id|String|Somente leitura.|
|isDefault|Booliano|Indica se este é o arquivo de contrato padrão se nenhuma das culturas corresponder à preferência do cliente. Se nenhum dos arquivos estiver marcado como padrão, o primeiro será tratado como o padrão. Somente leitura.|
|idioma|Cadeia de caracteres|Cultura do arquivo de contrato no formato languagecode2-Country/regioncode2. languagecode2 é um código de duas letras em minúsculas derivado de ISO 639-1. Country/regioncode2 é derivado de ISO 3166 e geralmente consiste em duas letras maiúsculas ou uma marca de idioma BCP-47 (por exemplo, en-US). Somente leitura.|
|isMajorVersion|Boolean|Indica se o arquivo de contrato é uma atualização de versão principal. As atualizações de versão principal invalidam as aceitação do contrato no idioma correspondente. |
|createdDateTime|DateTimeOffset|A data e hora que representam o momento em que o arquivo foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.|

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


