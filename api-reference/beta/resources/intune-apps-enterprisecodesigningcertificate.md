---
title: tipo de recurso de enterpriseCodeSigningCertificate
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75e02555f6e9af5283e0a727d34725458c1d99a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406721"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>tipo de recurso de enterpriseCodeSigningCertificate

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista enterpriseCodeSigningCertificates](../api/intune-apps-enterprisecodesigningcertificate-list.md)|coleção [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Lista as propriedades e os relacionamentos dos objetos [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Obter enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Leia as propriedades e os relacionamentos do objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Criar enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-create.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Crie um novo objeto de [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Excluir enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-delete.md)|Nenhum|Exclui um [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).|
|[Atualizar enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Atualize as propriedades de um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade.|
|content|Binária|O certificado de assinatura de código de empresa do Windows no formato de dados brutos.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|O Status do certificado provisionado ou não foi provisionado. Os valores possíveis são: `notProvisioned` e `provisioned`.|
|SubjectName|Cadeia de caracteres|O nome do assunto para o cert.|
|subject|String|O valor de assunto para o cert.|
|issuerName|String|O nome do emissor para o cert.|
|emissor|String|O valor de emissor para o cert.|
|expirationDateTime|DateTimeOffset|A data de validade do Cert.|
|uploadDateTime|DateTimeOffset|A data hora de certificado de assinatura de código padrão quando ele é carregado.|

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




