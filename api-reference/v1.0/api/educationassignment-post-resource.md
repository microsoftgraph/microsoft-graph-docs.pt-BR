---
title: Criar educationAssignmentResource
description: Criar um recurso de atribuição de educação.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 43489a196136daaa7fcefd51664dce366d798cb2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128809"
---
# <a name="create-educationassignmentresource"></a>Criar educationAssignmentResource

Namespace: microsoft.graph

Criar um [recurso de atribuição](../resources/educationassignmentresource.md). Você pode criar os seguintes tipos de recursos de atribuição:

- [educationFileResource](../resources/educationfileresource.md)
- [educationExcelResource](../resources/educationexcelresource.md)
- [educationWordResource](../resources/educationwordresource.md)
- [educationLinkResource](../resources/educationlinkresource.md)
- [educationPowerPointResource](../resources/educationpowerpointresource.md)
- [educationMediaResource](../resources/educationmediaresource.md)

Cada recurso tem uma propriedade @odata.type para indicar qual tipo de recurso está sendo criado. 

> [!IMPORTANT] 
> Antes de carregar um recurso de atribuição, você deve configurar a pasta [de](../api/educationassignment-setupresourcesfolder.md) recursos para o [educationAssignment](../resources/educationassignment.md) para carregar os arquivos.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | Sem suporte.  | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{class-id}/assignments/{assignment-id}/resources
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um dos seguintes tipos de recurso: 

- [educationFileResource](../resources/educationfileresource.md)
- [educationExcelResource](../resources/educationexcelresource.md)
- [educationWordResource](../resources/educationwordresource.md)
- [educationLinkResource](../resources/educationlinkresource.md)
- [educationPowerPointResource](../resources/educationpowerpointresource.md)
- [educationMediaResource](../resources/educationmediaresource.md)

>**Observação:** Você não pode usar essa operação para criar [um educationExternalResource](../resources/educationexternalresource.md).

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="example-1-create-an-educationlinkresource"></a>Exemplo 1: Criar um educationLinkResource
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80"],  
  "name": "create_educationlinkresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources
Content-type: application/json

{
    "distributeForStudentWork": false,
    "resource": {
        "displayName": "Where the Wonders of Learning Never Cease | Wonderopolis",
        "link": "https://wonderopolis.org/",
        "thumbnailPreviewUrl": null,
        "@odata.type": "#microsoft.graph.educationLinkResource"
    }
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationLinkResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
  "assignmentResourceUrl": null,  
    "id": "a2f95693-aea2-4d5e-a936-11ef390f8f20",
    "resource": {
        "@odata.type": "#microsoft.graph.educationLinkResource",
        "displayName": "Where the Wonders of Learning Never Cease | Wonderopolis",
        "createdDateTime": "2021-09-13T15:50:39.0017937Z",
        "lastModifiedDateTime": "2021-09-13T15:50:39.0017937Z",
        "link": "https://wonderopolis.org/",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-2-create-an-educationwordresource"></a>Exemplo 2: Criar um educationWordResource
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80"],  
  "name": "create_educationwordresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources
Content-type: application/json

{
    "distributeForStudentWork":false,
    "resource": {
        "@odata.type": "microsoft.graph.educationWordResource",
        "displayName": "Issues and PR in guthub.docx",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2"
                                          
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationwordresource-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationwordresource-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationwordresource-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationwordresource-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-educationwordresource-from-educationassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-educationwordresource-from-educationassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationWordResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "assignmentResourceUrl": null,
    "id": "d835503f-fd00-4840-b69c-7230d10e18b8",
    "resource": {
        "@odata.type": "#microsoft.graph.educationWordResource",
        "displayName": "Issues and PR in guthub.docx",
        "createdDateTime": "2021-08-04T00:23:08.6269586Z",
        "lastModifiedDateTime": "2021-08-04T00:23:08.6269586Z",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-3-create-an-educationfileresource"></a>Exemplo 3: Criar um educationFileResource
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80"],  
  "name": "create_educationfileresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources
Content-type: application/json

{
    "distributeForStudentWork":false,
    "resource": {
        "displayName": "article.pdf",
        "file": {
            "odataid": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RPHKSP6THE4ORD2RQAR6MQLF26G"
        },
        "@odata.type": "#microsoft.graph.educationFileResource"
    }
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
                                                                                       

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

                                                                                                                                                                                         

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "eec7f642-9d9a-406f-bbae-4b3b2c12e273",
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "displayName": "article.pdf",
        "createdDateTime": "2021-07-16T23:41:53.9378423Z",
        "lastModifiedDateTime": "2021-07-16T23:41:53.9378423Z",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeU6BLWBcGc_R6UgCKyYyTin/items/016XPCQEA5VVDIMU4BSFG3VBI37MPHZ3OE",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-4-create-an-educationexcelresource"></a>Exemplo 4: Criar um educationExcelResource
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80"], 
  "name": "create_educationexcelresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources
Content-type: application/json

{
    "distributeForStudentWork":false,
    "resource": {
        "@odata.type": "microsoft.graph.educationExcelResource",
        "displayName":"Graph Doc pages.xlsx",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationexcelresource-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationexcelresource-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationexcelresource-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationexcelresource-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-educationexcelresource-from-educationassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-educationexcelresource-from-educationassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationExcelResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "assignmentResourceUrl": null,
    "id": "517b36a6-9ca2-4e7b-9748-3af25f5cd4fd",
    "resource": {
        "@odata.type": "#microsoft.graph.educationExcelResource",
        "displayName": "Graph Doc pages.xlsx",
        "createdDateTime": "2021-09-13T15:50:49.7107759Z",
        "lastModifiedDateTime": "2021-09-13T15:50:49.7107759Z",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-5-create-an-educationpowerpointresource"></a>Exemplo 5: Criar um educationPowerPointResource
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80"], 
  "name": "create_educationpowerpointresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources
Content-type: application/json

{
    "distributeForStudentWork":false,
    "resource": {
        "@odata.type": "microsoft.graph.educationPowerPointResource",
        "displayName":"state diagram.pptx",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationpowerpointresource-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationpowerpointresource-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationpowerpointresource-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationpowerpointresource-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-educationpowerpointresource-from-educationassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-educationpowerpointresource-from-educationassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPowerPointResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
  "assignmentResourceUrl": null,
    "id": "3cb7968b-082f-4756-bdfb-782b4538cc0a",
    "resource": {
        "@odata.type": "#microsoft.graph.educationPowerPointResource",
    "displayName": "state diagram.pptx",
        "createdDateTime": "2021-09-13T15:50:58.5428117Z",
        "lastModifiedDateTime": "2021-09-13T15:50:58.5428117Z",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```

### <a name="example-6-create-an-educationmediaresource"></a>Exemplo 6: Criar um educationMediaResource
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1618dfb0-3ff2-4edf-8d5c-b8f81df00e80"], 
  "name": "create_educationmediaresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources
Content-type: application/json

{
    "distributeForStudentWork":false,
    "resource": {
        "@odata.type": "microsoft.graph.educationMediaResource",
        "displayName":"homework example.PNG",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationmediaresource-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationmediaresource-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationmediaresource-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationmediaresource-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-educationmediaresource-from-educationassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-educationmediaresource-from-educationassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationMediaResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "30495bfd-c912-49d5-b3e1-92b60db3142a",
    "resource": {
        "@odata.type": "#microsoft.graph.educationMediaResource",
        "displayName": "homework example.PNG",
        "createdDateTime": "2021-09-16T00:09:32.2133895Z",
        "lastModifiedDateTime": "2021-09-16T00:09:32.2133895Z",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                "displayName": null
            }
        }
    }
}
```


## <a name="see-also"></a>Confira também

* [Estados, transições e limitações para atribuições e envios](/graph/assignments-submissions-states-transition)
* [Upload arquivos para atribuições e envios de educação](/graph/education-upload-resource-overview)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


