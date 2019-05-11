---
title: tipo de recurso iosEduCertificateSettings
description: Certificados de raiz confiável e PFX para iOS EDU.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4305745c8b9d12bf19c4e8be6c10f24076ec29f1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946501"
---
# <a name="ioseducertificatesettings-resource-type"></a>tipo de recurso iosEduCertificateSettings

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Certificados de raiz confiável e PFX para iOS EDU.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|trustedRootCertificate|Binária|Certificado raiz confiável.|
|certFileName|Cadeia de caracteres|Nome do arquivo a ser exibido na interface do usuário.|
|certificationAuthority|Cadeia de caracteres|Autoridade de certificação PKCS.|
|certificationAuthorityName|Cadeia de caracteres|Nome da autoridade de certificação PKCS.|
|certificateTemplateName|Cadeia de caracteres|Nome do modelo de certificado PKCS.|
|renewalThresholdPercentage|Int32|Porcentagem de limite de renovação de certificado. Valores válidos de 1 a 99|
|certificateValidityPeriodValue|Int32|Valor para o período de validade do certificado.|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Dimensionar o período de validade do certificado. Os valores possíveis são: `days`, `months`, `years`.|

## <a name="relationships"></a>Relações
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




