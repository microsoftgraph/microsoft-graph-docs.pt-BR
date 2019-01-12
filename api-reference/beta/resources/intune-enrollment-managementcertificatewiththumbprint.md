---
title: tipo de recurso de managementCertificateWithThumbprint
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6e6259c1f90547ff875fa31d3f383606749bc0dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983349"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a>tipo de recurso de managementCertificateWithThumbprint

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|impressão digital|Cadeia de caracteres|A impressão digital do certificado gerenciamento|
|certificado|Cadeia de caracteres|O certificado de gerenciamento codificada de Base 64|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```





