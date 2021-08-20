---
title: Tipo de recurso iosEduCertificateSettings
description: Certificados Raiz confiável e PFX para iOS EDU.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 35e630422185164c14c86073803b752cd98ccf7f48e3608bd504a760074cf8e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248520"
---
# <a name="ioseducertificatesettings-resource-type"></a>Tipo de recurso iosEduCertificateSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Certificados Raiz confiável e PFX para iOS EDU.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|trustedRootCertificate|Binário|Certificado Raiz Confiável.|
|certFileName|Cadeia de caracteres|Nome do arquivo a ser exibido na interface do usuário.|
|certificationAuthority|Cadeia de caracteres|Autoridade de Certificação PKCS.|
|certificationAuthorityName|Cadeia de caracteres|Nome da Autoridade de Certificação PKCS.|
|certificateTemplateName|Cadeia de caracteres|Nome do modelo de certificado PKCS.|
|renewalThresholdPercentage|Int32|Porcentagem de limite de renovação de certificado. Valores válidos de 1 a 99|
|certificateValidityPeriodValue|Int32|Valor do Período de Validade do Certificado.|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Dimensione para o Período de Validade do Certificado. Os valores possíveis são: `days`, `months`, `years`.|

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




