---
title: tipo de recurso enterpriseCodeSigningCertificate
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac5f5a901e147523e1da8d14d0d782603b02cdd7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157166"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>tipo de recurso enterpriseCodeSigningCertificate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar enterpriseCodeSigningCertificates](../api/intune-apps-enterprisecodesigningcertificate-list.md)|coleção [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Listar Propriedades e relações dos objetos [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Obter enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Leia as propriedades e as relações do objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Criar enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-create.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Criar um novo objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Excluir enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-delete.md)|Nenhum|Exclui [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).|
|[Atualizar enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Atualiza as propriedades de um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da entidade.|
|content|Binária|O certificado de assinatura de código do Windows Enterprise no formato de dados brutos.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|O status do certificado provisionado ou não foi provisionado. Os valores possíveis são: `notProvisioned` e `provisioned`.|
|SubjectName|String|O nome da entidade do certificado.|
|subject|String|O valor de entidade para o certificado.|
|issuerName|String|O nome do emissor do certificado.|
|emissor|String|O valor do emissor para o certificado.|
|expirationDateTime|DateTimeOffset|A data de expiração do certificado.|
|uploadDateTime|DateTimeOffset|A data/hora do certificado de codeSignação quando é carregado.|

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




