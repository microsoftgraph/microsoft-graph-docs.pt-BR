---
title: tipo de recurso de iosEduCertificateSettings
description: Certificados raiz e PFX confiáveis para iOS EDU.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bf6b0da4d3ff7af562ae99e81e10f52351bd735d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822075"
---
# <a name="ioseducertificatesettings-resource-type"></a>tipo de recurso de iosEduCertificateSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Certificados raiz e PFX confiáveis para iOS EDU.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|trustedRootCertificate|Binária|Certificado raiz confiável.|
|Nome_arquivo_cert|Cadeia de caracteres|Nome de arquivo a ser exibido na interface do usuário.|
|certificationAuthority|Cadeia de caracteres|Autoridade de certificação PKCS.|
|certificationAuthorityName|Cadeia de caracteres|Nome da autoridade de certificação PKCS.|
|certificateTemplateName|Cadeia de caracteres|Nome do modelo de certificado PKCS.|
|renewalThresholdPercentage|Int32|Porcentagem de limite de renovação de certificados. Valores válidos 1 a 99|
|certificateValidityPeriodValue|Int32|Valor para o período de validade do certificado.|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Escala para o período de validade do certificado. Os valores possíveis são: `days`, `months`, `years`.|

## <a name="relationships"></a>Relacionamentos
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```





