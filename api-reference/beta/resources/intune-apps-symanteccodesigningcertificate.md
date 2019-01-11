---
title: tipo de recurso de symantecCodeSigningCertificate
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a2e4f53e0ca7329f163b507677e2b91a4c02fe12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845007"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>tipo de recurso de symantecCodeSigningCertificate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Leia as propriedades e os relacionamentos do objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .|
|[Atualizar symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Atualize as propriedades de um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade.|
|content|Binária|O certificado de assinatura de código do Windows Symantec no formato de dados brutos.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|O Status de Cert provisionado ou não foi provisionado. Os valores possíveis são: `notProvisioned` e `provisioned`.|
|password|Cadeia de caracteres|A senha necessária para o arquivo. pfx.|
|SubjectName|Cadeia de caracteres|O nome do assunto para o cert.|
|subject|Cadeia de caracteres|O valor de assunto para o cert.|
|issuerName|Cadeia de caracteres|O nome do emissor para o cert.|
|emissor|Cadeia de caracteres|O valor de emissor para o cert.|
|expirationDateTime|DateTimeOffset|A data de validade do Cert.|
|uploadDateTime|DateTimeOffset|O tipo do certificado de assinatura de código padrão como Symantec Cert.|

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





