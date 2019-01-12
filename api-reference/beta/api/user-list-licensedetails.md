---
title: Listar licenseDetails
description: Recupere uma lista de objetos licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80b2e707ec6106def7d8539dcf5e8e9a20179503
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991892"
---
# <a name="list-licensedetails"></a><span data-ttu-id="844ab-103">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="844ab-103">List licenseDetails</span></span>

> <span data-ttu-id="844ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="844ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="844ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="844ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="844ab-106">Recupere uma lista de objetos licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="844ab-106">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="844ab-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="844ab-107">Permissions</span></span>
<span data-ttu-id="844ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="844ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="844ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="844ab-110">Permission type</span></span>      | <span data-ttu-id="844ab-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="844ab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="844ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="844ab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="844ab-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="844ab-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="844ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="844ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="844ab-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="844ab-115">User.Read</span></span>    |
|<span data-ttu-id="844ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="844ab-116">Application</span></span> | <span data-ttu-id="844ab-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="844ab-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="844ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="844ab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="844ab-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="844ab-119">Optional query parameters</span></span>
<span data-ttu-id="844ab-120">Esse método **não** suporta [Parâmetros da Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="844ab-120">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="844ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="844ab-121">Request headers</span></span>
| <span data-ttu-id="844ab-122">Nome</span><span class="sxs-lookup"><span data-stu-id="844ab-122">Name</span></span>      |<span data-ttu-id="844ab-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="844ab-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="844ab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="844ab-124">Authorization</span></span>  | <span data-ttu-id="844ab-125">&lt;Código&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="844ab-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="844ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="844ab-126">Request body</span></span>
<span data-ttu-id="844ab-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="844ab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="844ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="844ab-128">Response</span></span>

<span data-ttu-id="844ab-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [licenseDetails](../resources/licensedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="844ab-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="844ab-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="844ab-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="844ab-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="844ab-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="844ab-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="844ab-132">Response</span></span>
<span data-ttu-id="844ab-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="844ab-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
