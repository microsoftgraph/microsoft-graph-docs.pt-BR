---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5606906cbec0122137faf3cb454edec785c42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405797"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a>Tipo de recurso windowsInformationProtectionDataRecoveryCertificate

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

DataRecoveryCertificate da proteção de informações do Windows

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|SubjectName|Cadeia de caracteres|Nome do assunto do certificado de recuperação de dados|
|descrição|Cadeia de caracteres|Descrição do certificado de recuperação de dados|
|expirationDateTime|DateTimeOffset|Datetime de vencimento do certificado de recuperação de dados|
|certificado|Binário|Certificado de recuperação de dados|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```




