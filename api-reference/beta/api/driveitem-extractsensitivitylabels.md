---
title: 'driveItem: extractSensitivityLabels'
description: Extraia um ou mais rótulos de confidencialidade atribuídos a um item de unidade.
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d516f6f530041d662f6818d5f8d832762678b038
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208880"
---
# <a name="driveitem-extractsensitivitylabels"></a>driveItem: extractSensitivityLabels
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Extraia um ou mais rótulos de confidencialidade atribuídos a um item de unidade e atualize os metadados de um item de unidade com os detalhes mais recentes do rótulo atribuído. Em caso de falha ao extrair os rótulos de confidencialidade de um arquivo, um erro de extração será gerado com o código de erro e a mensagem aplicáveis.

> **Observação**: essa API é aplicável somente para extensões de arquivo com suporte. Quando chamada, essa API recupera primeiro os metadados do rótulo de confidencialidade do arquivo do banco de dados e, em seguida, verifica se os detalhes do rótulo de confidencialidade são os mais recentes em termos de conteúdo do arquivo. Se sim, os valores recuperados do banco de dados serão retornados. Se não, os rótulos de confidencialidade serão extraídos do fluxo de conteúdo do arquivo, os metadados correspondentes serão atualizados no banco de dados e os valores recém-extraídos serão retornados.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                             |
|:--------------------------------------|:--------------------------------------------------------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All                                        |
|Aplicativo                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All                                |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drive-id}/items/{item-id}/extractSensitivityLabels
POST /drives/{drive-id}/root:/{item-path}/extractSensitivityLabels
POST /groups/{group-id}/drive/items/{item-id}/extractSensitivityLabels
POST /groups/{group-id}/drive/root:/{item-path}/extractSensitivityLabels
POST /me/drive/items/{item-id}/extractSensitivityLabels
POST /me/drive/root:/{item-path}/extractSensitivityLabels
POST /sites/{site-id}/drive/items/{item-id}/extractSensitivityLabels
POST /sites/{site-id}/drive/root:/{item-path}/extractSensitivityLabels
POST /users/{user-id}/drive/items/{item-id}/extractSensitivityLabels
POST /users/{user-id}/drive/root:/{item-path}/extractSensitivityLabels
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um objeto [extractSensitivityLabelsResult](../resources/extractsensitivitylabelsresult.md) no corpo da resposta.

Além dos erros gerais que se aplicam ao Microsoft Graph, essa API `423 Locked` retorna o código de resposta, que indica que o arquivo que está sendo acessado está bloqueado. Nesses casos, a propriedade **de código** do objeto de resposta indica o tipo de erro que bloqueia a extração do rótulo de confidencialidade.
A seguir estão os valores possíveis para os tipos de erro.

| Valor                       | Descrição                                                                                                         |
|:----------------------------|:--------------------------------------------------------------------------------------------------------------------|
| fileDoubleKeyEncrypted      | Indica que o arquivo está protegido por meio da criptografia de chave dupla; portanto, ele não pode ser aberto para a extração dos rótulos de confidencialidade.             |
| fileDecryptionNotSupported  | Indica que o arquivo criptografado tem propriedades específicas que não permitem que esses arquivos sejam abertos pelo SharePoint extrair rótulos de confidencialidade.    |
| fileDecryptionDeferred      | Indica que o arquivo está sendo processado para descriptografia; portanto, ele não pode ser aberto para a extração dos rótulos de confidencialidade.      |
| unknownFutureValue          | Valor de sentinel de enumeração evolvável. Não usar.                                                                   |

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "extract-sensitivitylabels", "tags": "service.graph" } -->
``` http
POST https://graph.microsoft.com/beta/drive/root/items/016GVDAP3RCQS5VBQHORFIVU2ZMOSBL25U/extractSensitivityLabels
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/extract-sensitivitylabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/extract-sensitivitylabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extractSensitivityLabelsResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "microsoft.graph.extractSensitivityLabelsResult",
    "labels": [
      {
        "sensitivityLabelId": "5feba255-812e-446a-ac59-a7044ef827b5",
        "assignmentMethod": "standard",
        "tenantId": "fed495cb-8c27-41ea-8749-00b0a084bc3d"
      },
      {
        "sensitivityLabelId": "fa781fdf-68c8-43ec-ae08-c4813deb2144",
        "assignmentMethod": "standard",
        "tenantId": "277601b1-6094-456c-a358-95bfc99539d7"
      },
      {
        "sensitivityLabelId": "3937098d-df0c-4c8d-8f66-5876b57b75ba",
        "assignmentMethod": "standard",
        "tenantId": "f2477f30-c8a2-422d-8995-6f056b494655"
      }
    ]
  }
}
```

