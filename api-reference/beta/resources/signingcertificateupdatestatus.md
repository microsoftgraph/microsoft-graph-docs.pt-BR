---
title: Tipo de recurso signingCertificateUpdateStatus
description: Fornece o status da última atualização do certificado de autenticação.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 108b5169ac9b043e4ce2a80f5c620a266d391338
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2022
ms.locfileid: "64852650"
---
# <a name="signingcertificateupdatestatus-resource-type"></a>Tipo de recurso signingCertificateUpdateStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece o status e o carimbo de data/hora da última atualização do certificado de assinatura. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|certificateUpdateResult|Cadeia de caracteres|Status da última atualização do certificado. Somente leitura. Para obter uma lista de status, consulte [o status certificateUpdateResult](#certificateupdateresult-status).|
|lastRunDateTime|DateTimeOffset|Data e hora no formato ISO 8601 e na hora UTC em que o certificado foi atualizado pela última vez. Somente leitura. |

### <a name="certificateupdateresult-status"></a>Status de certificateUpdateResult
| Valor | Descrição |
| :--- | :--- |
|sucesso|A operação de atualização de certificado foi bem-sucedida.|
|Unknownerror|O motivo da falha é indefinido.|
|internalServerError|Ocorreu um erro interno do servidor ao processar a solicitação.|
|noValidExistingCertFound|Nenhum certificado de autenticação existente válido foi encontrado.|
|noStsAuthUrlFound|Nenhuma URL de autenticação sts foi encontrada.|
|noFederationProtocolFound|O protocolo de federação foi indefinido.|
|noNewCertificateFound|Nenhum novo certificado foi encontrado.|
|couldNotAccessRemoteHost|Não foi possível acessar o provedor para obter os novos certificados.|
|connectionError|Ocorreu um erro de conexão, por exemplo, um tempo limite de conexão.|
|xmlParsingError|Falha ao analisar o XML.|
|badRequest|Recebeu um código `400 BadRequest` de erro na solicitação de metadados alimentados.|
|Desautorizado|Código `401 Unauthorized` de erro recebido na solicitação de metadados alimentados.|
|Proibido|Código `403 Forbidden` de erro recebido na solicitação de metadados alimentados.|
|Notfound|Código `404 NotFound` de erro recebido na solicitação de metadados alimentados.|
|providerError|Recebeu um `500 InternalServerError` código de erro do provedor.|


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

