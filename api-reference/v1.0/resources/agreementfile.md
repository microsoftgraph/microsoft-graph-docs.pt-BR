---
title: Tipo de recurso agreementFile
description: Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: dee599f1639df5f5255fa4852de29f52bc0b6907
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650661"
---
# <a name="agreementfile-resource-type"></a>Tipo de recurso agreementFile

Namespace: microsoft.graph

Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).

Herda de [agreementFileProperties](agreementfileproperties.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|A data que representa quando o arquivo foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Herdado [de agreementFileProperties](../resources/agreementfileproperties.md).|
|displayName|String|Nome de exibição localizado do arquivo de política de um contrato. O nome de exibição localizado é mostrado aos usuários finais que visualizam o contrato. Herdado [de agreementFileProperties](../resources/agreementfileproperties.md).|
|fileData|[agreementFileData](agreementfiledata.md)|Dados que representam os termos de uso do documento PDF. Somente leitura. Herdado [de agreementFileProperties](../resources/agreementfileproperties.md).|
|fileName|String|Nome do arquivo de contrato (por exemplo, TOU.pdf). Somente leitura. Herdado [de agreementFileProperties](../resources/agreementfileproperties.md).|
|id|String|O identificador do objeto agreementFileVersion. Somente leitura. Herdado [de agreementFileProperties](../resources/agreementfileproperties.md).|
|isDefault|Booliano|Se nenhum dos idiomas corresponde à preferência do cliente, indica se esse é o arquivo de contrato padrão . Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão. Somente leitura. Herdado [de agreementFileProperties](../resources/agreementfileproperties.md).|
|isMajorVersion|Booliano|Indica se o arquivo de contrato é uma atualização de versão principal. Atualizações de versão principais invalidam as aceitaçãos do contrato no idioma correspondente. Herdado [de agreementFileProperties](../resources/agreementfileproperties.md).|
|idioma|Cadeia de caracteres|O idioma do arquivo de contrato no formato "languagecode2-country/regioncode2". "languagecode2" é um código de duas letras minúsculo derivado da ISO 639-1, enquanto "country/regioncode2" é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47. Por exemplo, inglês dos EUA é `en-US` . Somente leitura. Herdado [de agreementFileProperties](../resources/agreementfileproperties.md).|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|localizações|[Coleção agreementFileLocalization](agreementfilelocalization.md)|A versão localizada dos arquivos de contrato de uso anexados ao contrato.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.agreementFile",
  "keyProperty": "id"
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


