---
title: Obter educationSchool
description: Recupere as propriedades e relações do objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 72788c938f7beccd79622731f437a99b07aaec9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324832"
---
# <a name="get-educationschool"></a><span data-ttu-id="ec259-103">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="ec259-103">Get educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec259-104">Recupere as propriedades e relações do objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="ec259-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec259-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec259-105">Permissions</span></span>
<span data-ttu-id="ec259-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec259-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec259-108">Permission type</span></span>      | <span data-ttu-id="ec259-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec259-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec259-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec259-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ec259-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ec259-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="ec259-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec259-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ec259-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec259-113">Not supported.</span></span>  |
|<span data-ttu-id="ec259-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec259-114">Application</span></span> | <span data-ttu-id="ec259-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec259-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ec259-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec259-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec259-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec259-117">Optional query parameters</span></span>
<span data-ttu-id="ec259-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec259-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec259-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec259-119">Request headers</span></span>
| <span data-ttu-id="ec259-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec259-120">Header</span></span>       | <span data-ttu-id="ec259-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ec259-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec259-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec259-122">Authorization</span></span>  | <span data-ttu-id="ec259-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec259-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec259-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec259-125">Request body</span></span>
<span data-ttu-id="ec259-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec259-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ec259-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec259-127">Response</span></span>
<span data-ttu-id="ec259-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec259-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec259-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec259-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec259-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec259-130">Request</span></span>
<span data-ttu-id="ec259-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec259-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10001
```
##### <a name="response"></a><span data-ttu-id="ec259-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec259-132">Response</span></span>
<span data-ttu-id="ec259-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec259-133">The following is an example of the response.</span></span> 

><span data-ttu-id="ec259-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec259-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "schoolPrincipalEmail": "AmyRoebuck@contoso.com",
  "schoolPrincipalName": "Amy Roebuck",
  "externalSchoolPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
