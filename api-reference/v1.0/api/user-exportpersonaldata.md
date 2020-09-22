---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar os dados de um usuário organizacional.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: bd61c123bf566b97a926c6db81169b704e9f0b93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992150"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="b4a72-103">usuário: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="b4a72-103">user: exportPersonalData</span></span>

<span data-ttu-id="b4a72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4a72-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4a72-105">Envie uma solicitação de operação de política de dados de um administrador da empresa ou de um aplicativo para exportar os dados de um usuário organizacional.</span><span class="sxs-lookup"><span data-stu-id="b4a72-105">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4a72-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4a72-106">Permissions</span></span>
<span data-ttu-id="b4a72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4a72-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4a72-109">Permission type</span></span>      | <span data-ttu-id="b4a72-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4a72-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4a72-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4a72-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b4a72-112">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="b4a72-112">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="b4a72-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4a72-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b4a72-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="b4a72-114">Not applicable</span></span>  |
|<span data-ttu-id="b4a72-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4a72-115">Application</span></span> | <span data-ttu-id="b4a72-116">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="b4a72-116">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="b4a72-117">**Observação:** A exportação só pode ser realizada por um administrador da empresa quando permissões delegadas são usadas.</span><span class="sxs-lookup"><span data-stu-id="b4a72-117">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="b4a72-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4a72-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="b4a72-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a72-119">Request headers</span></span>
| <span data-ttu-id="b4a72-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b4a72-120">Name</span></span>       | <span data-ttu-id="b4a72-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4a72-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b4a72-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4a72-122">Authorization</span></span>  | <span data-ttu-id="b4a72-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b4a72-123">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4a72-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a72-124">Request body</span></span>
<span data-ttu-id="b4a72-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4a72-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b4a72-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b4a72-126">Parameter</span></span>    | <span data-ttu-id="b4a72-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4a72-127">Type</span></span>   |<span data-ttu-id="b4a72-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4a72-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4a72-129">storageLocation</span><span class="sxs-lookup"><span data-stu-id="b4a72-129">storageLocation</span></span>|<span data-ttu-id="b4a72-130">String</span><span class="sxs-lookup"><span data-stu-id="b4a72-130">String</span></span>|<span data-ttu-id="b4a72-131">Esta é uma URL de assinatura de acesso compartilhado (SAS) para uma conta de armazenamento do Azure, onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="b4a72-131">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="b4a72-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4a72-132">Response</span></span>
<span data-ttu-id="b4a72-133">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="b4a72-133">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="b4a72-134">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4a72-134">It does not return anything in the response body.</span></span> <span data-ttu-id="b4a72-135">A resposta contém os cabeçalhos de resposta a seguir.</span><span class="sxs-lookup"><span data-stu-id="b4a72-135">The response contains the following response headers.</span></span>

| <span data-ttu-id="b4a72-136">Nome</span><span class="sxs-lookup"><span data-stu-id="b4a72-136">Name</span></span>       | <span data-ttu-id="b4a72-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4a72-137">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b4a72-138">Local</span><span class="sxs-lookup"><span data-stu-id="b4a72-138">Location</span></span>  | <span data-ttu-id="b4a72-139">URL para verificar o status da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4a72-139">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="b4a72-140">Repetir-após</span><span class="sxs-lookup"><span data-stu-id="b4a72-140">Retry-After</span></span>  | <span data-ttu-id="b4a72-141">Período de tempo em segundos.</span><span class="sxs-lookup"><span data-stu-id="b4a72-141">Time period in seconds.</span></span> <span data-ttu-id="b4a72-142">O criador de solicitação deve aguardar esse tempo depois de enviar uma solicitação para verificar o status.</span><span class="sxs-lookup"><span data-stu-id="b4a72-142">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="b4a72-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4a72-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4a72-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a72-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b4a72-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4a72-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b4a72-146">C#</span><span class="sxs-lookup"><span data-stu-id="b4a72-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4a72-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4a72-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4a72-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4a72-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4a72-149">Java</span><span class="sxs-lookup"><span data-stu-id="b4a72-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-exportpersonaldata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b4a72-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4a72-150">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
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

