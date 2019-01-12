---
title: Listar licenseDetails
description: Recupere uma lista de objetos licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ad9b10a377e89858cad03d3eabe4e62a4f86627
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931822"
---
# <a name="list-licensedetails"></a><span data-ttu-id="2de59-103">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="2de59-103">List licenseDetails</span></span>

<span data-ttu-id="2de59-104">Recupere uma lista de objetos licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="2de59-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2de59-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2de59-105">Permissions</span></span>
<span data-ttu-id="2de59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2de59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2de59-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2de59-108">Permission type</span></span>      | <span data-ttu-id="2de59-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2de59-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2de59-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2de59-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2de59-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2de59-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2de59-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2de59-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2de59-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="2de59-113">User.Read</span></span>    |
|<span data-ttu-id="2de59-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2de59-114">Application</span></span> | <span data-ttu-id="2de59-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de59-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2de59-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2de59-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2de59-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2de59-117">Optional query parameters</span></span>
<span data-ttu-id="2de59-118">Esse método **não** suporta [Parâmetros da Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="2de59-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2de59-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2de59-119">Request headers</span></span>
| <span data-ttu-id="2de59-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2de59-120">Name</span></span>      |<span data-ttu-id="2de59-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2de59-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2de59-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2de59-122">Authorization</span></span>  | <span data-ttu-id="2de59-123">&lt;Código&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="2de59-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="2de59-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2de59-124">Request body</span></span>
<span data-ttu-id="2de59-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2de59-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2de59-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2de59-126">Response</span></span>

<span data-ttu-id="2de59-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [licenseDetails](../resources/licensedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2de59-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2de59-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2de59-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2de59-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2de59-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="2de59-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2de59-130">Response</span></span>
<span data-ttu-id="2de59-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2de59-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
