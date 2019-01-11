---
title: 'page: copyToSection'
description: Copia uma página para uma seção específica.
localization_priority: Normal
ms.openlocfilehash: 10d0eecd2f84a33e66209f8297b72b8a4630b100
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892502"
---
# <a name="page-copytosection"></a><span data-ttu-id="f2b57-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="f2b57-103">page: copyToSection</span></span>

> <span data-ttu-id="f2b57-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2b57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2b57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2b57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2b57-106">Copia uma página para uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="f2b57-106">Copies a page to a specific section.</span></span>

<span data-ttu-id="f2b57-107">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="f2b57-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2b57-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2b57-108">Permissions</span></span>
<span data-ttu-id="f2b57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2b57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2b57-111">Permission type</span></span>      | <span data-ttu-id="f2b57-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2b57-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2b57-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2b57-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f2b57-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b57-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2b57-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2b57-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2b57-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2b57-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f2b57-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2b57-117">Application</span></span> | <span data-ttu-id="f2b57-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b57-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2b57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b57-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="f2b57-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b57-120">Request headers</span></span>
| <span data-ttu-id="f2b57-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f2b57-121">Name</span></span>       | <span data-ttu-id="f2b57-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2b57-122">Type</span></span> | <span data-ttu-id="f2b57-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2b57-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2b57-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2b57-124">Authorization</span></span>  | <span data-ttu-id="f2b57-125">string</span><span class="sxs-lookup"><span data-stu-id="f2b57-125">string</span></span>  | <span data-ttu-id="f2b57-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2b57-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2b57-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2b57-128">Content-Type</span></span> | <span data-ttu-id="f2b57-129">string</span><span class="sxs-lookup"><span data-stu-id="f2b57-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f2b57-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b57-130">Request body</span></span>
<span data-ttu-id="f2b57-131">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.</span><span class="sxs-lookup"><span data-stu-id="f2b57-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="f2b57-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f2b57-132">Parameter</span></span>    | <span data-ttu-id="f2b57-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2b57-133">Type</span></span>   |<span data-ttu-id="f2b57-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2b57-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2b57-135">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="f2b57-135">siteCollectionId</span></span>|<span data-ttu-id="f2b57-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2b57-136">String</span></span>|<span data-ttu-id="f2b57-137">A identificação do site do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="f2b57-137">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="f2b57-138">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f2b57-138">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="f2b57-139">siteId</span><span class="sxs-lookup"><span data-stu-id="f2b57-139">siteId</span></span>|<span data-ttu-id="f2b57-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2b57-140">String</span></span>|<span data-ttu-id="f2b57-141">A identificação da web do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="f2b57-141">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="f2b57-142">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f2b57-142">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="f2b57-143">groupId</span><span class="sxs-lookup"><span data-stu-id="f2b57-143">groupId</span></span>|<span data-ttu-id="f2b57-144">String</span><span class="sxs-lookup"><span data-stu-id="f2b57-144">String</span></span>|<span data-ttu-id="f2b57-p106">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f2b57-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="f2b57-147">id</span><span class="sxs-lookup"><span data-stu-id="f2b57-147">id</span></span>|<span data-ttu-id="f2b57-148">String</span><span class="sxs-lookup"><span data-stu-id="f2b57-148">String</span></span>|<span data-ttu-id="f2b57-p107">Obrigatório. A id da seção de destino.</span><span class="sxs-lookup"><span data-stu-id="f2b57-p107">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="f2b57-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2b57-151">Response</span></span>

<span data-ttu-id="f2b57-p108">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="f2b57-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="f2b57-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2b57-154">Example</span></span>
<span data-ttu-id="f2b57-155">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f2b57-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f2b57-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b57-156">Request</span></span>
<span data-ttu-id="f2b57-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2b57-157">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f2b57-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2b57-158">Response</span></span>
<span data-ttu-id="f2b57-159">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2b57-159">Here is an example of the response.</span></span>
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
