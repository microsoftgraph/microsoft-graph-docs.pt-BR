---
title: Lista educationAssignmentResources
description: Obtenha todos os recursos associados a essa atribuição.
ms.openlocfilehash: 2092b7a98794bc8eaeac7e65eea5dced8ffa00d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035888"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="8c79a-103">Lista educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="8c79a-103">List educationAssignmentResources</span></span>

> <span data-ttu-id="8c79a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8c79a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c79a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8c79a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c79a-106">Obtenha todos os recursos associados a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="8c79a-106">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c79a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8c79a-107">Permissions</span></span>
<span data-ttu-id="8c79a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c79a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c79a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c79a-110">Permission type</span></span>      | <span data-ttu-id="8c79a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c79a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c79a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c79a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="8c79a-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c79a-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8c79a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c79a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8c79a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c79a-115">Not supported.</span></span>  |
|<span data-ttu-id="8c79a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c79a-116">Application</span></span> | <span data-ttu-id="8c79a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c79a-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8c79a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c79a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c79a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8c79a-119">Optional query parameters</span></span>
<span data-ttu-id="8c79a-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8c79a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c79a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c79a-121">Request headers</span></span>
| <span data-ttu-id="8c79a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c79a-122">Header</span></span>       | <span data-ttu-id="8c79a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8c79a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c79a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c79a-124">Authorization</span></span>  | <span data-ttu-id="8c79a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c79a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c79a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c79a-127">Request body</span></span>
<span data-ttu-id="8c79a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c79a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8c79a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c79a-129">Response</span></span>
<span data-ttu-id="8c79a-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c79a-130">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c79a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c79a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c79a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c79a-132">Request</span></span>
<span data-ttu-id="8c79a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c79a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="8c79a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c79a-134">Response</span></span>
<span data-ttu-id="8c79a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8c79a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8c79a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c79a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
      "resource": {
          "@odata.type": "#microsoft.graph.educationWordResource",
          "displayName": "Report.docx",
          "createdDateTime": "2017-10-21T07:52:53.9863696Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
      },
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
