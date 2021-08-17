---
title: Tipo de recurso vppTokenLicenseSummary
description: Resumo da licença de um determinado aplicativo em um token.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9bba6090a415eb2eab5cb2607668f850b64c2b70a32e329d63ce9d77b0a2f28d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54161112"
---
# <a name="vpptokenlicensesummary-resource-type"></a>Tipo de recurso vppTokenLicenseSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo da licença de um determinado aplicativo em um token.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|vppTokenId|Cadeia de caracteres|Identificador do token VPP.|
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




