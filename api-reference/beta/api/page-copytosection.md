---
title: 'page: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: dd7abb016345195bd5a32e20a5623d6fca9fd6ff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516438"
---
# <a name="page-copytosection"></a><span data-ttu-id="b23ce-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="b23ce-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b23ce-104">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="b23ce-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="b23ce-105">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="b23ce-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="b23ce-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b23ce-106">Permissions</span></span>
<span data-ttu-id="b23ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b23ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b23ce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b23ce-109">Permission type</span></span>      | <span data-ttu-id="b23ce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b23ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b23ce-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b23ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b23ce-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23ce-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b23ce-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b23ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b23ce-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b23ce-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b23ce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b23ce-115">Application</span></span> | <span data-ttu-id="b23ce-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23ce-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b23ce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b23ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="b23ce-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b23ce-118">Request headers</span></span>
| <span data-ttu-id="b23ce-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b23ce-119">Name</span></span>       | <span data-ttu-id="b23ce-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b23ce-120">Type</span></span> | <span data-ttu-id="b23ce-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b23ce-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b23ce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b23ce-122">Authorization</span></span>  | <span data-ttu-id="b23ce-123">string</span><span class="sxs-lookup"><span data-stu-id="b23ce-123">string</span></span>  | <span data-ttu-id="b23ce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b23ce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b23ce-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b23ce-126">Content-Type</span></span> | <span data-ttu-id="b23ce-127">string</span><span class="sxs-lookup"><span data-stu-id="b23ce-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b23ce-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b23ce-128">Request body</span></span>
<span data-ttu-id="b23ce-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.</span><span class="sxs-lookup"><span data-stu-id="b23ce-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="b23ce-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b23ce-130">Parameter</span></span>    | <span data-ttu-id="b23ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b23ce-131">Type</span></span>   |<span data-ttu-id="b23ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b23ce-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b23ce-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="b23ce-133">siteCollectionId</span></span>|<span data-ttu-id="b23ce-134">String</span><span class="sxs-lookup"><span data-stu-id="b23ce-134">String</span></span>|<span data-ttu-id="b23ce-135">A identificação do site do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="b23ce-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="b23ce-136">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b23ce-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b23ce-137">siteId</span><span class="sxs-lookup"><span data-stu-id="b23ce-137">siteId</span></span>|<span data-ttu-id="b23ce-138">String</span><span class="sxs-lookup"><span data-stu-id="b23ce-138">String</span></span>|<span data-ttu-id="b23ce-139">A identificação da web do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="b23ce-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="b23ce-140">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b23ce-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b23ce-141">groupId</span><span class="sxs-lookup"><span data-stu-id="b23ce-141">groupId</span></span>|<span data-ttu-id="b23ce-142">String</span><span class="sxs-lookup"><span data-stu-id="b23ce-142">String</span></span>|<span data-ttu-id="b23ce-p105">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b23ce-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="b23ce-145">id</span><span class="sxs-lookup"><span data-stu-id="b23ce-145">id</span></span>|<span data-ttu-id="b23ce-146">String</span><span class="sxs-lookup"><span data-stu-id="b23ce-146">String</span></span>|<span data-ttu-id="b23ce-p106">Obrigatório. A id da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="b23ce-p106">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="b23ce-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b23ce-149">Response</span></span>

<span data-ttu-id="b23ce-p107">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="b23ce-p107">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b23ce-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b23ce-152">Example</span></span>
<span data-ttu-id="b23ce-153">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b23ce-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b23ce-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b23ce-154">Request</span></span>
<span data-ttu-id="b23ce-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b23ce-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="b23ce-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b23ce-156">Response</span></span>
<span data-ttu-id="b23ce-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b23ce-157">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
