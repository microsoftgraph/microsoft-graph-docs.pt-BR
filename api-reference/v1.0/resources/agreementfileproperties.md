---
title: Tipo de recurso agreementFileProperties
description: Representa as propriedades de um arquivo de contrato de uso; incluindo o idioma localizado e o nome de exibição.
author: raprakasMSFT
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e3c5ac4199d603f336c10dc732bc2f54110f7a3a
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650770"
---
# <a name="agreementfileproperties-resource-type"></a>Tipo de recurso agreementFileProperties

Namespace: microsoft.graph

Representa as propriedades de um arquivo de contrato de uso; incluindo o idioma localizado e o nome de exibição.

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|A data que representa quando o arquivo foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|displayName|String|Nome de exibição localizado do arquivo de política de um contrato. O nome de exibição localizado é mostrado aos usuários finais que visualizam o contrato.|
|fileData|[agreementFileData](agreementfiledata.md)|Dados que representam os termos de uso do documento PDF. Somente leitura.|
|fileName|String|Nome do arquivo de contrato (por exemplo, TOU.pdf). Somente leitura.|
|id|String|O identificador do objeto agreementFileVersion. Somente leitura.|
|isDefault|Booliano|Se nenhum dos idiomas corresponde à preferência do cliente, indica se esse é o arquivo de contrato padrão . Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão. Somente leitura.|
|isMajorVersion|Booliano|Indica se o arquivo de contrato é uma atualização de versão principal. Atualizações de versão principais invalidam as aceitaçãos do contrato no idioma correspondente.|
|idioma|Cadeia de caracteres|O idioma do arquivo de contrato no formato "languagecode2-country/regioncode2". "languagecode2" é um código de duas letras minúsculo derivado da ISO 639-1, enquanto "country/regioncode2" é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47. Por exemplo, inglês dos EUA é `en-US` . Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreementFileProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreementFileProperties",
  "id": "String (identifier)",
  "fileName": "String",
  "language": "String",
  "isDefault": "Boolean",
  "isMajorVersion": "Boolean",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "fileData": {
    "@odata.type": "microsoft.graph.agreementFileData"
  }
}
```

