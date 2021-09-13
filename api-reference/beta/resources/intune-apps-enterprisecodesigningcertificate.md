---
title: Tipo de recurso enterpriseCodeSigningCertificate
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3ba7fd4b46359c10778b4f040701aff7411e87aa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064571"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>Tipo de recurso enterpriseCodeSigningCertificate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar enterpriseCodeSigningCertificates](../api/intune-apps-enterprisecodesigningcertificate-list.md)|[coleção enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Listar propriedades e relações dos [objetos enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)|
|[Obter enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Ler propriedades e relações do [objeto enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)|
|[Criar enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-create.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Crie um novo [objeto enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)|
|[Excluir enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-delete.md)|Nenhum|Exclui um [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).|
|[Atualizar enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Atualize as propriedades de [um objeto enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da entidade.|
|conteúdo|Binário|O Windows Enterprise Code-Signing certificado no formato de dados brutos.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|O Status do Certificado Provisionado ou não Provisionado. Os valores possíveis são: `notProvisioned` e `provisioned`.|
|SubjectName|Cadeia de caracteres|O Nome do Assunto do certificado.|
|assunto|Cadeia de caracteres|O Valor do Assunto do certificado.|
|issuerName|Cadeia de caracteres|O Nome do Emissor do certificado.|
|emissor|String|O valor emissor do certificado.|
|expirationDateTime|DateTimeOffset|A Data de Expiração do Certificado.|
|uploadDateTime|DateTimeOffset|A data em que CodeSigning Cert é carregado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enterpriseCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```



