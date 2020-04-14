---
title: tipo de recurso androidEnrollmentCompanyCode
description: Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b380ea8b085b0328b166b6f9ba0f65bf5df4af76
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459288"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>tipo de recurso androidEnrollmentCompanyCode

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enrollmentToken|String|Token de registro usado pelo usuário para registrar seus dispositivos.|
|qrCodeContent|String|Cadeia de caracteres usada para gerar um código QR para o token.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Código QR gerado para o token.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



