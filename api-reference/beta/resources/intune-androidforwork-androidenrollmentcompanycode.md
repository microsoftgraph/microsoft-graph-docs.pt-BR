---
title: Tipo de recurso androidEnrollmentCompanyCode
description: Uma classe para manter dados de registro especializados usados para o registro por meio da API de Gerenciamento do Android do Google, como Token, Url e conteúdo de código QR
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6803a04883d90d3550b98582522e74465251d96f803896d55e62afff5ad9f58a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54173328"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>Tipo de recurso androidEnrollmentCompanyCode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe para manter dados de registro especializados usados para o registro por meio da API de Gerenciamento do Android do Google, como Token, Url e conteúdo de código QR

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enrollmentToken|Cadeia de caracteres|Token de Registro usado pelo Usuário para registrar seu dispositivo.|
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




