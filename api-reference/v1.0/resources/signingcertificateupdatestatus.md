---
title: Tipo de recurso signingCertificateUpdateStatus
description: Fornece o status da última atualização do certificado de autenticação.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 59129a7ce9d523c17fd4d497e91bf20da7af10b0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447395"
---
# <a name="signingcertificateupdatestatus-resource-type"></a>Tipo de recurso signingCertificateUpdateStatus

Namespace: microsoft.graph

Fornece o status e o carimbo de data/hora da última atualização do certificado de assinatura. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|certificateUpdateResult|Cadeia de caracteres|Status da última atualização do certificado. Somente leitura. Para obter uma lista de status, consulte [o status certificateUpdateResult](#certificateupdateresult-status).|
|lastRunDateTime|DateTimeOffset|Data e hora no formato ISO 8601 e na hora UTC em que o certificado foi atualizado pela última vez. Somente leitura. |

### <a name="certificateupdateresult-status"></a>Status de certificateUpdateResult
| Valor | Descrição |
| :--- | :--- |
|sucesso|A tentativa foi bem-sucedida.|
|Unknownerror|Não sei o motivo da falha.|
|internalServerError|Algo deu errado do nosso lado.|
|noValidExistingCertFound|Nenhum certificado de autenticação existente válido foi encontrado.|
|noStsAuthUrlFound|Nenhuma URL de Autenticação STS foi encontrada.|
|noFederationProtocolFound|Nenhum protocolo de federação foi encontrado.|
|noNewCertificateFound|Nenhum novo certificado foi encontrado.|
|couldNotAccessRemoteHost|Não foi possível acessar o provedor para obter os novos certificados.|
|connectionError|Erro de conexão|
|xmlParsingError|Falha ao analisar o XML|
|badRequest|Erro BadRequest recebido da solicitação de metadados alimentados.|
|Desautorizado|Erro não autorizado recebido da solicitação de metadados alimentados.|
|Proibido|Erro Recebido Proibido da solicitação de metadados alimentados.|
|Notfound|Erro NotFound recebido da solicitação de metadados alimentados.|
|providerError|Recebido InternalServerError do provedor.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.signingCertificateUpdateStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signingCertificateUpdateStatus",
  "certificateUpdateResult": "String",
  "lastRunDateTime": "String (timestamp)"
}
```

