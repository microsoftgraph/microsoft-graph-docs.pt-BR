---
title: Tipo de recurso agreementFileLocalization
description: Representa um arquivo de política localizado de um contrato de termos de uso no Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 6a1e68914d6e8d12d6777505036a0132ceac151685c5a5723d0581434cbe7b0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169687"
---
# <a name="agreementfilelocalization-resource-type"></a>Tipo de recurso agreementFileLocalization

Namespace: microsoft.graph

Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|Dados que representam os termos de uso do documento PDF. Apenas leitura.|
|fileName|String|Nome do arquivo de contrato (por exemplo, TOU.pdf). Somente leitura.|
|id|Cadeia de caracteres|O identificador do objeto agreementFileLocalization. Somente leitura.|
|isDefault|Booliano| Se nenhum dos idiomas corresponde à preferência do cliente, indica que esse é o arquivo de contrato padrão. Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão. Somente leitura.|
|idioma|Cadeia de caracteres|O idioma do arquivo de contrato no formato languagecode2-country/regioncode2. languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1. country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US). Somente leitura.|
|isMajorVersion|Booliano|Indica se o arquivo de contrato é uma atualização de versão principal. Atualizações de versão principais invalidam as aceitaçãos do contrato no idioma correspondente. |
|createdDateTime|DateTimeOffset|A data que representa quando o arquivo foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.|
|displayName|Cadeia de caracteres|Nome de exibição localizado do arquivo de política de um contrato. O nome de exibição localizado é mostrado aos usuários finais que visualizam o contrato.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileLocalization"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": "Boolean",
  "language": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
