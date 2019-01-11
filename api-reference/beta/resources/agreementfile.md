---
title: tipo de recurso de agreementFile
description: Representa um termos personalizável do arquivo do contrato de uso que gerencia de um inquilino com o Azure Active Directory (AD Azure). Ele contém metadados sobre o arquivo do contrato (por exemplo, o nome, o idioma, e se ele está o arquivo padrão).
localization_priority: Normal
ms.openlocfilehash: f06792d63deabf25659a09e8aec5ed0e8f036472
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804505"
---
# <a name="agreementfile-resource-type"></a>tipo de recurso de agreementFile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um termos personalizável do arquivo do contrato de uso que gerencia de um inquilino com o Azure Active Directory (AD Azure). Ele contém metadados sobre o arquivo do contrato (por exemplo, o nome, o idioma, e se ele está o arquivo padrão).

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
|fileData|[agreementFileData](agreementfiledata.md)|Dados que representam as condições de usar o documento PDF. Somente leitura.|
|fileName|Cadeia de caracteres|Nome do arquivo contrato (por exemplo, TOU.pdf). Somente leitura.|
|id|Cadeia de caracteres|Somente leitura.|
|isDefault|Booliano|Indica se esse é o arquivo padrão do contrato se nenhuma das culturas corresponder a preferência do cliente. Se nenhum dos arquivos estiverem marcados como padrão, primeiro será tratado como padrão. Somente leitura.|
|idioma|Cadeia de caracteres|Cultura do arquivo no formato languagecode2-país/regioncode2 contrato. languagecode2 é um código de duas letras minúsculas, derivado do ISO 639-1. País/regioncode2 é derivado do ISO 3166 e normalmente consiste em duas letras maiusculas ou uma marca de idioma BCP-47 (por exemplo, en-US). Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
