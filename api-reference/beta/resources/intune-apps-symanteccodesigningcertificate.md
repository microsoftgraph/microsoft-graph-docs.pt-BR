---
title: Tipo de recurso symantecCodeSigningCertificate
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 817911afa2d18a0c0dc50a1f98afbbe412f7aba9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783999"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>Tipo de recurso symantecCodeSigningCertificate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Leia propriedades e relações do [objeto symantecCodeSigningCertificate.](../resources/intune-apps-symanteccodesigningcertificate.md)|
|[Atualizar symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Atualize as propriedades de um [objeto symantecCodeSigningCertificate.](../resources/intune-apps-symanteccodesigningcertificate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade.|
|conteúdo|Binário|O Windows Symantec Code-Signing Certificado no formato de dados brutos.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|O Status do Certificado Provisionado ou não Provisionado. Os valores possíveis são: `notProvisioned` e `provisioned`.|
|password|String|A senha necessária para o arquivo .pfx.|
|SubjectName|Cadeia de caracteres|O Nome do Assunto do certificado.|
|assunto|Cadeia de caracteres|O valor Subject do certificado.|
|issuerName|Cadeia de caracteres|O Nome do Emissor do certificado.|
|emissor|Cadeia de caracteres|O valor emissor do certificado.|
|expirationDateTime|DateTimeOffset|A Data de Expiração do Certificado.|
|uploadDateTime|DateTimeOffset|O Tipo do Certificado de Design de Código como Certificado Symantec.|

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



