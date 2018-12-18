---
title: tipo de recurso de vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
author: tfitzmac
ms.openlocfilehash: 7847c6265ed526d50215567918698c7732adf947
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319975"
---
# <a name="vpptokenlicensesummary-resource-type"></a>tipo de recurso de vppTokenLicenseSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Resumo de licenças de um determinado aplicativo em um token.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|vppTokenId|String|Identificador do token VPP.|
|appleId|Cadeia de caracteres|O Apple Id associado ao Token do Programa de Compra de Volume da Apple.|
|organizationName|Cadeia de caracteres|A organização associada com o Token de programa de compra de Volume Apple.|
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





