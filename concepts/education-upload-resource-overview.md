---
title: Carregar arquivos para tarefas e envios educacionais
description: Saiba como carregar um arquivo em uma tarefa ou um recurso de envio usando a API de educação no Microsoft Graph.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: f6c3f9a3a35e89ed935105e6320c4f7c652b288f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440870"
---
# <a name="upload-files-for-education-assignments-and-submissions-using-the-microsoft-graph-api"></a>Carregar arquivos para tarefas e envios de educação usando o Microsoft API do Graph

Os recursos são uma parte integrante das tarefas [e envios](/graph/api/resources/educationassignment) [educacionais](/graph/api/resources/educationsubmission). Os professores determinam os recursos a serem carregados em uma pasta de tarefas e os alunos determinam os recursos a serem carregados em uma pasta de envio.

Este artigo descreve como usar a API de educação no Microsoft Graph para carregar arquivos em uma pasta de atribuição ou envio.

## <a name="prerequisites"></a>Pré-requisitos

Antes de carregar arquivos, configure uma pasta do SharePoint para a qual carregar os arquivos para uma determinada atribuição de educação ou recurso de envio.

## <a name="upload-a-resource"></a>Carregar um recurso

A `setUpResourcesFolder` API retorna um modelo que contém a **propriedade resourcesFolderUrl** .

```http
{
    ...
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GFA"
    ...
}
```

As etapas a seguir descrevem como carregar um recurso/arquivo em uma pasta de recursos relevante.

### <a name="step-1---construct-the-upload-url"></a>Etapa 1 – Construir a URL de upload
Crie a URL para carregar conteúdo seguindo este formato específico `{resourcesFolderUrl}:/{Name of new file}:/content`. O exemplo a seguir mostra uma URL de upload que contém **a propriedade resourcesFolderUrl** .

```http
https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2:/MyPictureFile.png:/content
```

### <a name="step-2---upload-the-resource-to-sharepoint"></a>Etapa 2 – Carregar o recurso no SharePoint
Faça uma solicitação PUT com a URL de upload para carregar o conteúdo.

O conteúdo do corpo da solicitação deve ser o fluxo binário do arquivo a ser carregado.

Para obter mais detalhes, consulte [Carregar arquivos grandes com uma sessão de upload](/graph/api/driveitem-createuploadsession).

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação.

```http
PUT https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2:/MyPictureFile.png:/content
Content-Type: text/plain

Binary data for the file
```

#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#drives('b%216SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F')/items/$entity",
    "@microsoft.graph.downloadUrl": "...",
    "createdDateTime": "2021-03-11T18:49:47Z",
    "eTag": "\"{EDD00CE7-B74C-4C3E-BA3E-484CB41EF31D},1\"",
    "id": "01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
    "lastModifiedDateTime": "2021-03-11T18:49:47Z",
    "name": "MyPictureFile.png",
    "webUrl": "https://contososdorg.sharepoint.com/sites/GraphTest/Class%20Files/Assignments/Test%20File%20Distribution/MyPictureFile.png",
    "cTag": "\"c:{EDD00CE7-B74C-4C3E-BA3E-484CB41EF31D},2\"",
    "size": 2302233,
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "email": "t-james@contososd.org",
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": "James"
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "email": "t-james@contososd.org",
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": "James"
        }
    },
    "parentReference": {
        "driveId": "b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F",
        "driveType": "documentLibrary",
        "id": "01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2",
        "path": "/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/root:/Assignments/Test File Distribution"
    },
    "file": {
        "mimeType": "image/png",
        "hashes": {
            "quickXorHash": "CvYQxN7MCGrIsdrA38c6wWhOu5g="
        }
    },
    "fileSystemInfo": {
        "createdDateTime": "2021-03-11T18:49:47Z",
        "lastModifiedDateTime": "2021-03-11T18:49:47Z"
    },
    "image": {}
}
```

### <a name="step-3---construct-the-value-for-the-fileurl-property"></a>Etapa 3 – Construir o valor para a propriedade fileUrl
Crie o valor para a **propriedade fileUrl** usando o seguinte formato: `https://graph.microsoft.com/v1.0/drives/{drive-id}/items/{item-id}`. Substitua os `{drive-id}` espaços `{item-id}` reservados e os valores descritos na tabela a seguir.

| Espaço reservado | Descrição | Exemplo |
|:--|:--|:--|
| `{drive-id}` | ID da unidade da URL de solicitação usada na etapa 2. | b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F |
| `{item-id}` | ID do item do corpo da resposta obtido na etapa 2. | 01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ |

O exemplo a seguir mostra **um fileUrl** com base nesse formato.

```http
https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ
```

### <a name="step-4---create-educationassignmentresource"></a>Etapa 4 – Criar educationAssignmentResource
Esta etapa mostra como carregar um recurso do SharePoint em uma pasta de recursos de atribuição.

Use a `fileUrl` etapa anterior no corpo da solicitação para [Criar um educationAssignmentResource](/graph/api/educationassignment-post-resources).

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação.

```http
POST https://graph.microsoft.com/v1.0/education/classes/b07edbef-7420-4b3d-8f7c-d599cf21e069/assignments/48b80dff-452a-4108-bd85-fa0d84e39d0a/resources
Content-type: application/json

{
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
        "displayName": "Parts of a Sonnet"
    }
}
```

#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('48b80dff-452a-4108-bd85-fa0d84e39d0a')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "ff1aafe4-ae89-49c3-8366-4b509f640d6a",
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "displayName": "Parts of a Sonnet",
        "createdDateTime": "2021-03-11T18:35:40.6642039Z",
        "lastModifiedDateTime": "2021-03-11T18:35:40.6642039Z",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
                "displayName": null
            }
        }
    }
}
```

Agora você carregou com êxito um recurso do SharePoint em uma pasta de recursos de atribuição (e o anexou à atribuição associada). Você pode seguir etapas semelhantes para carregar um ou mais recursos de trabalho do aluno.

Para obter mais detalhes, [consulte Create educationSubmissionResource](/graph/api/educationsubmission-post-resources).
