---
title: tipo de recurso iosEduCertificateSettings
description: Certificados de raiz confiável e PFX para iOS EDU.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b7c3c545f65ffd019d4d3eefe672f9a665bbd41f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463015"
---
# <a name="ioseducertificatesettings-resource-type"></a>tipo de recurso iosEduCertificateSettings

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Certificados de raiz confiável e PFX para iOS EDU.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|trustedRootCertificate|Binária|Certificado raiz confiável.|
|certFileName|String|Nome do arquivo a ser exibido na interface do usuário.|
|certificationAuthority|String|Autoridade de certificação PKCS.|
|certificationAuthorityName|String|Nome da autoridade de certificação PKCS.|
|certificateTemplateName|String|Nome do modelo de certificado PKCS.|
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



