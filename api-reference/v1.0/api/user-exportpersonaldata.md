---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar os dados de um usuário organizacional.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cd36bc4af64c244612ef60b1693d3603200dc975
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278033"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="2c8ad-103">usuário: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="2c8ad-103">user: exportPersonalData</span></span>

<span data-ttu-id="2c8ad-104">Envie uma solicitação de operação de política de dados de um administrador da empresa ou de um aplicativo para exportar os dados de um usuário organizacional.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c8ad-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c8ad-105">Permissions</span></span>
<span data-ttu-id="2c8ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c8ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c8ad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c8ad-108">Permission type</span></span>      | <span data-ttu-id="2c8ad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c8ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c8ad-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c8ad-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2c8ad-111">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="2c8ad-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="2c8ad-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c8ad-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2c8ad-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="2c8ad-113">Not applicable</span></span>  |
|<span data-ttu-id="2c8ad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c8ad-114">Application</span></span> | <span data-ttu-id="2c8ad-115">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="2c8ad-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="2c8ad-116">**Observação:** A exportação só pode ser realizada por um administrador da empresa quando permissões delegadas são usadas.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="2c8ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c8ad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="2c8ad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8ad-118">Request headers</span></span>
| <span data-ttu-id="2c8ad-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2c8ad-119">Name</span></span>       | <span data-ttu-id="2c8ad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8ad-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2c8ad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c8ad-121">Authorization</span></span>  | <span data-ttu-id="2c8ad-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2c8ad-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c8ad-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8ad-123">Request body</span></span>
<span data-ttu-id="2c8ad-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2c8ad-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2c8ad-125">Parameter</span></span>    | <span data-ttu-id="2c8ad-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c8ad-126">Type</span></span>   |<span data-ttu-id="2c8ad-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8ad-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c8ad-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="2c8ad-128">storageLocation</span></span>|<span data-ttu-id="2c8ad-129">String</span><span class="sxs-lookup"><span data-stu-id="2c8ad-129">String</span></span>|<span data-ttu-id="2c8ad-130">Esta é uma URL de assinatura de acesso compartilhado (SAS) para uma conta de armazenamento do Azure, onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="2c8ad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c8ad-131">Response</span></span>
<span data-ttu-id="2c8ad-132">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="2c8ad-133">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-133">It does not return anything in the response body.</span></span> <span data-ttu-id="2c8ad-134">A resposta contém os cabeçalhos de resposta a seguir.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-134">The response contains the following response headers.</span></span>

| <span data-ttu-id="2c8ad-135">Nome</span><span class="sxs-lookup"><span data-stu-id="2c8ad-135">Name</span></span>       | <span data-ttu-id="2c8ad-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8ad-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2c8ad-137">Locais</span><span class="sxs-lookup"><span data-stu-id="2c8ad-137">Location</span></span>  | <span data-ttu-id="2c8ad-138">URL para verificar o status da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-138">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="2c8ad-139">Repetir-após</span><span class="sxs-lookup"><span data-stu-id="2c8ad-139">Retry-After</span></span>  | <span data-ttu-id="2c8ad-140">Período de tempo em segundos.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-140">Time period in seconds.</span></span> <span data-ttu-id="2c8ad-141">O criador de solicitação deve aguardar esse tempo depois de enviar uma solicitação para verificar o status.</span><span class="sxs-lookup"><span data-stu-id="2c8ad-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="2c8ad-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c8ad-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c8ad-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8ad-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a><span data-ttu-id="2c8ad-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c8ad-144">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c8ad-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c8ad-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c8ad-146">C#</span><span class="sxs-lookup"><span data-stu-id="2c8ad-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c8ad-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c8ad-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c8ad-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2c8ad-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
