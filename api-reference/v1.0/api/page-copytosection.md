---
title: 'page: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
ms.openlocfilehash: 971d5eb47c6130ab7379e8b7db67d355b55c8d7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871495"
---
# <a name="page-copytosection"></a><span data-ttu-id="05744-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="05744-103">page: copyToSection</span></span>
<span data-ttu-id="05744-104">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="05744-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="05744-105">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="05744-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="05744-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05744-106">Permissions</span></span>
<span data-ttu-id="05744-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05744-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05744-109">Permission type</span></span>      | <span data-ttu-id="05744-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05744-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05744-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05744-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05744-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05744-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="05744-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05744-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05744-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05744-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="05744-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05744-115">Application</span></span> | <span data-ttu-id="05744-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05744-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05744-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05744-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="05744-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05744-118">Request headers</span></span>
| <span data-ttu-id="05744-119">Nome</span><span class="sxs-lookup"><span data-stu-id="05744-119">Name</span></span>       | <span data-ttu-id="05744-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="05744-120">Type</span></span> | <span data-ttu-id="05744-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="05744-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="05744-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="05744-122">Authorization</span></span>  | <span data-ttu-id="05744-123">string</span><span class="sxs-lookup"><span data-stu-id="05744-123">string</span></span>  | <span data-ttu-id="05744-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05744-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05744-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05744-126">Content-Type</span></span> | <span data-ttu-id="05744-127">string</span><span class="sxs-lookup"><span data-stu-id="05744-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="05744-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05744-128">Request body</span></span>
<span data-ttu-id="05744-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.</span><span class="sxs-lookup"><span data-stu-id="05744-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="05744-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="05744-130">Parameter</span></span>    | <span data-ttu-id="05744-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05744-131">Type</span></span>   |<span data-ttu-id="05744-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05744-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05744-133">groupId</span><span class="sxs-lookup"><span data-stu-id="05744-133">groupId</span></span>|<span data-ttu-id="05744-134">String</span><span class="sxs-lookup"><span data-stu-id="05744-134">String</span></span>|<span data-ttu-id="05744-p103">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="05744-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="05744-137">id</span><span class="sxs-lookup"><span data-stu-id="05744-137">id</span></span>|<span data-ttu-id="05744-138">String</span><span class="sxs-lookup"><span data-stu-id="05744-138">String</span></span>|<span data-ttu-id="05744-p104">Obrigatório. A id da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="05744-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="05744-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="05744-141">Response</span></span>

<span data-ttu-id="05744-p105">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="05744-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="05744-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05744-144">Example</span></span>
<span data-ttu-id="05744-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="05744-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="05744-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05744-146">Request</span></span>
<span data-ttu-id="05744-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05744-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="05744-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="05744-148">Response</span></span>
<span data-ttu-id="05744-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05744-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
