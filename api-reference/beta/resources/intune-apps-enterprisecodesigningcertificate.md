---
title: tipo de recurso de enterpriseCodeSigningCertificate
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: f16dbbf59af238e631e282d7e4d92dad46a7083b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328697"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>tipo de recurso de enterpriseCodeSigningCertificate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





