---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar os dados de um usuário organizacional.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 24262a733a4a8dcdc8724950b0c65bf31fdbc9a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067528"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="957b3-103">usuário: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="957b3-103">user: exportPersonalData</span></span>

<span data-ttu-id="957b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="957b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="957b3-105">Envia uma solicitação de operação de política de dados, realizada por um administrador da empresa para exportar os dados de um usuário da organização.</span><span class="sxs-lookup"><span data-stu-id="957b3-105">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="957b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="957b3-106">Permissions</span></span>
<span data-ttu-id="957b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="957b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="957b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="957b3-109">Permission type</span></span>      | <span data-ttu-id="957b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="957b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="957b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="957b3-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="957b3-112">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="957b3-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="957b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="957b3-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="957b3-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="957b3-114">Not applicable</span></span>  |
|<span data-ttu-id="957b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="957b3-115">Application</span></span> | <span data-ttu-id="957b3-116">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="957b3-116">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="957b3-117">**Observação:** A exportação só pode ser realizada por um administrador da empresa quando a permissão delegada é usada.</span><span class="sxs-lookup"><span data-stu-id="957b3-117">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="957b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="957b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="957b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="957b3-119">Request headers</span></span>
| <span data-ttu-id="957b3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="957b3-120">Name</span></span>       | <span data-ttu-id="957b3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="957b3-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="957b3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="957b3-122">Authorization</span></span>  | <span data-ttu-id="957b3-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="957b3-123">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="957b3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="957b3-124">Request body</span></span>
<span data-ttu-id="957b3-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="957b3-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="957b3-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="957b3-126">Parameter</span></span>    | <span data-ttu-id="957b3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="957b3-127">Type</span></span>   |<span data-ttu-id="957b3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="957b3-128">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="957b3-129">storageLocation</span><span class="sxs-lookup"><span data-stu-id="957b3-129">storageLocation</span></span>|<span data-ttu-id="957b3-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="957b3-130">String</span></span>|<span data-ttu-id="957b3-131">Esta é uma URL de assinatura de acesso compartilhado (SAS) para uma conta de armazenamento do Azure, onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="957b3-131">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="957b3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="957b3-132">Response</span></span>
<span data-ttu-id="957b3-133">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="957b3-133">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="957b3-134">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="957b3-134">It does not return anything in the response body.</span></span> <span data-ttu-id="957b3-135">A resposta contém os cabeçalhos a seguir.</span><span class="sxs-lookup"><span data-stu-id="957b3-135">The response contains the following headers.</span></span>

| <span data-ttu-id="957b3-136">Nome</span><span class="sxs-lookup"><span data-stu-id="957b3-136">Name</span></span>       | <span data-ttu-id="957b3-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="957b3-137">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="957b3-138">Local</span><span class="sxs-lookup"><span data-stu-id="957b3-138">Location</span></span>  | <span data-ttu-id="957b3-139">URL para verificar o status da solicitação.</span><span class="sxs-lookup"><span data-stu-id="957b3-139">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="957b3-140">Repetir-após</span><span class="sxs-lookup"><span data-stu-id="957b3-140">Retry-After</span></span>  | <span data-ttu-id="957b3-141">Período de tempo em segundos.</span><span class="sxs-lookup"><span data-stu-id="957b3-141">Time period in seconds.</span></span> <span data-ttu-id="957b3-142">O criador de solicitação deve aguardar esse tempo depois de enviar uma solicitação para verificar o status.</span><span class="sxs-lookup"><span data-stu-id="957b3-142">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="957b3-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="957b3-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="957b3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="957b3-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="957b3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="957b3-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
# <a name="c"></a>[<span data-ttu-id="957b3-146">C#</span><span class="sxs-lookup"><span data-stu-id="957b3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="957b3-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="957b3-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="957b3-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="957b3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="957b3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="957b3-149">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

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
  ]
}-->


