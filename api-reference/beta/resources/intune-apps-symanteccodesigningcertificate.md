---
title: tipo de recurso symantecCodeSigningCertificate
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99cdc636f0a8a5eb5381d09e7c3596bf3e41180d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012370"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>tipo de recurso symantecCodeSigningCertificate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Leia as propriedades e as relações do objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .|
|[Atualizar symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Atualiza as propriedades de um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da entidade.|
|conteúdo|Binária|O certificado de assinatura de código Symantec do Windows no formato de dados brutos.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|O status do certificado provisionado ou não foi provisionado. Os valores possíveis são: `notProvisioned` e `provisioned`.|
|password|String|A senha necessária para o arquivo. pfx.|
|SubjectName|Cadeia de caracteres|O nome da entidade do certificado.|
|subject|Cadeia de caracteres|O valor de entidade para o certificado.|
|issuerName|String|O nome do emissor do certificado.|
|emissor|String|O valor do emissor para o certificado.|
|expirationDateTime|DateTimeOffset|A data de expiração do certificado.|
|uploadDateTime|DateTimeOffset|O tipo do certificado de codesignação como CERT da Symantec.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```





