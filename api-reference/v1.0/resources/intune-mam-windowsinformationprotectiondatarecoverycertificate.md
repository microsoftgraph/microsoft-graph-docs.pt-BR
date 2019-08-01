---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 555cac098d2796f612054f11e2c5ade525ad6199
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037727"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a>Tipo de recurso windowsInformationProtectionDataRecoveryCertificate

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

DataRecoveryCertificate da proteção de informações do Windows

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|SubjectName|Cadeia de caracteres|Nome do assunto do certificado de recuperação de dados|
|descrição|String|Descrição do certificado de recuperação de dados|
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



