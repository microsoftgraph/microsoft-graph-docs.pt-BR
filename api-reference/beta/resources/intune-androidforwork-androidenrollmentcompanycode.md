---
title: Tipo de recurso androidEnrollmentCompanyCode
description: Uma classe para manter dados de registro especializados usados para o registro por meio da API de Gerenciamento do Android do Google, como Token, Url e conteúdo de código QR
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cef755a70e0dcb237196891d88a89aecad85015c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057639"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>Tipo de recurso androidEnrollmentCompanyCode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe para manter dados de registro especializados usados para o registro por meio da API de Gerenciamento do Android do Google, como Token, Url e conteúdo de código QR

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enrollmentToken|Cadeia de Caracteres|Token de Registro usado pelo Usuário para registrar seu dispositivo.|
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



