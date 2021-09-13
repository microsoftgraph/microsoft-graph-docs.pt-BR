---
title: Tipo de recurso vppTokenLicenseSummary
description: Resumo da licença de um determinado aplicativo em um token.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b442f7968c84f465a86e4ef1a0fc43353a957ac8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046712"
---
# <a name="vpptokenlicensesummary-resource-type"></a>Tipo de recurso vppTokenLicenseSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo da licença de um determinado aplicativo em um token.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|vppTokenId|Cadeia de Caracteres|Identificador do token VPP.|
|appleId|Cadeia de caracteres|O Apple Id associado ao Token do Programa de Compra de Volume da Apple.|
|organizationName|Cadeia de caracteres|A organização associada ao Token do Programa de Compra de Volume da Apple.|
|availableLicenseCount|Int32|O número de licenças VPP disponíveis.|
|usedLicenseCount|Int32|O número de aplicativos VPP em uso.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```



