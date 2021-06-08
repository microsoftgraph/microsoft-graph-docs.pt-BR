---
title: 'user: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um Administrador da Empresa para exportar dados de um usuário organizacional.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 56e42bbde7df9ea08405616eaab1342ac654e8eb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787718"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="07a5e-103">user: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="07a5e-103">user: exportPersonalData</span></span>

<span data-ttu-id="07a5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07a5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07a5e-105">Envie uma solicitação de operação de política de dados de um administrador da empresa ou de um aplicativo para exportar dados de um usuário organizacional.</span><span class="sxs-lookup"><span data-stu-id="07a5e-105">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="07a5e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="07a5e-106">Permissions</span></span>
<span data-ttu-id="07a5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07a5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07a5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07a5e-109">Permission type</span></span>      | <span data-ttu-id="07a5e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07a5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07a5e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07a5e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="07a5e-112">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="07a5e-112">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="07a5e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07a5e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="07a5e-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="07a5e-114">Not applicable</span></span>  |
|<span data-ttu-id="07a5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07a5e-115">Application</span></span> | <span data-ttu-id="07a5e-116">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="07a5e-116">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="07a5e-117">**Observação:** A exportação só pode ser executada por um administrador da empresa quando as permissões delegadas são usadas.</span><span class="sxs-lookup"><span data-stu-id="07a5e-117">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="07a5e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07a5e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="07a5e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07a5e-119">Request headers</span></span>
| <span data-ttu-id="07a5e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="07a5e-120">Name</span></span>       | <span data-ttu-id="07a5e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="07a5e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07a5e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07a5e-122">Authorization</span></span>  | <span data-ttu-id="07a5e-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="07a5e-123">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="07a5e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07a5e-124">Request body</span></span>
<span data-ttu-id="07a5e-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07a5e-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="07a5e-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="07a5e-126">Parameter</span></span>    | <span data-ttu-id="07a5e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="07a5e-127">Type</span></span>   |<span data-ttu-id="07a5e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="07a5e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07a5e-129">storageLocation</span><span class="sxs-lookup"><span data-stu-id="07a5e-129">storageLocation</span></span>|<span data-ttu-id="07a5e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a5e-130">String</span></span>|<span data-ttu-id="07a5e-131">Esta é uma URL de assinatura de acesso compartilhado (SAS) para uma conta Armazenamento do Azure, para onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="07a5e-131">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="07a5e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a5e-132">Response</span></span>
<span data-ttu-id="07a5e-133">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="07a5e-133">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="07a5e-134">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07a5e-134">It does not return anything in the response body.</span></span> <span data-ttu-id="07a5e-135">A resposta contém os seguintes headers de resposta.</span><span class="sxs-lookup"><span data-stu-id="07a5e-135">The response contains the following response headers.</span></span>

| <span data-ttu-id="07a5e-136">Nome</span><span class="sxs-lookup"><span data-stu-id="07a5e-136">Name</span></span>       | <span data-ttu-id="07a5e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="07a5e-137">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07a5e-138">Localização</span><span class="sxs-lookup"><span data-stu-id="07a5e-138">Location</span></span>  | <span data-ttu-id="07a5e-139">URL para verificar o status da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07a5e-139">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="07a5e-140">Retry-After</span><span class="sxs-lookup"><span data-stu-id="07a5e-140">Retry-After</span></span>  | <span data-ttu-id="07a5e-141">Período de tempo em segundos.</span><span class="sxs-lookup"><span data-stu-id="07a5e-141">Time period in seconds.</span></span> <span data-ttu-id="07a5e-142">O fazedor de solicitações deve aguardar tanto tempo depois de enviar uma solicitação para verificar o status.</span><span class="sxs-lookup"><span data-stu-id="07a5e-142">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="07a5e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07a5e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07a5e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07a5e-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="07a5e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="07a5e-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="07a5e-146">C#</span><span class="sxs-lookup"><span data-stu-id="07a5e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07a5e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07a5e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07a5e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07a5e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07a5e-149">Java</span><span class="sxs-lookup"><span data-stu-id="07a5e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-exportpersonaldata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07a5e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a5e-150">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```
<!-- {
  "blockType": "response",
  "truncated": true
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

