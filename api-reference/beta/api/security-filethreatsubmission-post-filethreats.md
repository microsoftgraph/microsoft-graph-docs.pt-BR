---
title: Criar fileThreatSubmission
description: Crie um novo objeto fileThreatSubmission.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9d90f57f4d40f461d98913078a294199b1b786be
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856462"
---
# <a name="create-filethreatsubmission"></a>Criar fileThreatSubmission
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto fileThreatSubmission](../resources/security-filethreatsubmission.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ThreatSubmission.ReadWrite,ThreatSubmission.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|ThreatSubmission.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/threatSubmission/fileThreats
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto fileContentThreatSubmission](../resources/security-filecontentthreatsubmission.md) . O [fileUrlContentThreatSubmission](../resources/security-fileurlthreatsubmission.md) está reservado e não tem suporte a partir de hoje.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto fileThreatSubmission](../resources/security-filethreatsubmission.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_filethreatsubmission_from_filethreats"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/threatSubmission/fileThreatSubmissions
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.fileContentThreatSubmission",
  "category": "malware",
  "fileName": "test.html",
  "fileContent": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.fileThreatSubmission"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/threatSubmission/fileThreatSubmission/$entity",
  "@odata.type": "#microsoft.graph.fileThreatSubmission",
  "category": "malware",
  "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
  "createdDateTime": "2021-10-10T03:30:18.6890937Z",
  "contentType": "file",
  "fileName": "test.html",
  "status": "running",
  "source": "administrator",
  "createdBy": {
    "user": {
      "identity": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin",
      "email": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com"
    }
  },
  "result": {
    "detail": "underInvestigation"
  },
  "adminReview": null,
  "tenantId" : "39238e87-b5ab-4ef6-a559-af54c6b07b42"
}
```

