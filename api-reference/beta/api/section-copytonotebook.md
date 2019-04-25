---
title: 'seção: copyToNotebook'
description: Copia uma seção para um bloco de anotações específico.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4ec5292aa7b11b268b73514af8aee42260e3d6a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545526"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="5e88b-103">seção: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="5e88b-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e88b-104">Copia uma seção para um bloco de anotações específico.</span><span class="sxs-lookup"><span data-stu-id="5e88b-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="5e88b-105">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="5e88b-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e88b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e88b-106">Permissions</span></span>
<span data-ttu-id="5e88b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e88b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e88b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e88b-109">Permission type</span></span>      | <span data-ttu-id="5e88b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e88b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e88b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e88b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e88b-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e88b-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e88b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e88b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e88b-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e88b-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5e88b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e88b-115">Application</span></span> | <span data-ttu-id="5e88b-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e88b-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e88b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e88b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="5e88b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e88b-118">Request headers</span></span>
| <span data-ttu-id="5e88b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5e88b-119">Name</span></span>       | <span data-ttu-id="5e88b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e88b-120">Type</span></span> | <span data-ttu-id="5e88b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e88b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5e88b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e88b-122">Authorization</span></span>  | <span data-ttu-id="5e88b-123">string</span><span class="sxs-lookup"><span data-stu-id="5e88b-123">string</span></span>  | <span data-ttu-id="5e88b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e88b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e88b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e88b-126">Content-Type</span></span> | <span data-ttu-id="5e88b-127">string</span><span class="sxs-lookup"><span data-stu-id="5e88b-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5e88b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e88b-128">Request body</span></span>
<span data-ttu-id="5e88b-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="5e88b-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="5e88b-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5e88b-130">Parameter</span></span>    | <span data-ttu-id="5e88b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e88b-131">Type</span></span>   |<span data-ttu-id="5e88b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e88b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e88b-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="5e88b-133">siteCollectionId</span></span>|<span data-ttu-id="5e88b-134">String</span><span class="sxs-lookup"><span data-stu-id="5e88b-134">String</span></span>|<span data-ttu-id="5e88b-135">A ID do site do SharePoint para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="5e88b-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="5e88b-136">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="5e88b-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="5e88b-137">siteId</span><span class="sxs-lookup"><span data-stu-id="5e88b-137">siteId</span></span>|<span data-ttu-id="5e88b-138">String</span><span class="sxs-lookup"><span data-stu-id="5e88b-138">String</span></span>|<span data-ttu-id="5e88b-139">A ID da Web do SharePoint a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="5e88b-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="5e88b-140">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="5e88b-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="5e88b-141">groupId</span><span class="sxs-lookup"><span data-stu-id="5e88b-141">groupId</span></span>|<span data-ttu-id="5e88b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e88b-142">String</span></span>|<span data-ttu-id="5e88b-143">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="5e88b-143">The id of the group to copy to.</span></span> <span data-ttu-id="5e88b-144">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="5e88b-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="5e88b-145">id</span><span class="sxs-lookup"><span data-stu-id="5e88b-145">id</span></span>|<span data-ttu-id="5e88b-146">String</span><span class="sxs-lookup"><span data-stu-id="5e88b-146">String</span></span>|<span data-ttu-id="5e88b-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e88b-147">Required.</span></span> <span data-ttu-id="5e88b-148">A ID do bloco de anotações de destino.</span><span class="sxs-lookup"><span data-stu-id="5e88b-148">The id of the destination notebook.</span></span> |
|<span data-ttu-id="5e88b-149">renomeas</span><span class="sxs-lookup"><span data-stu-id="5e88b-149">renameAs</span></span>|<span data-ttu-id="5e88b-150">String</span><span class="sxs-lookup"><span data-stu-id="5e88b-150">String</span></span>|<span data-ttu-id="5e88b-151">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="5e88b-151">The name of the copy.</span></span> <span data-ttu-id="5e88b-152">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="5e88b-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="5e88b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e88b-153">Response</span></span>

<span data-ttu-id="5e88b-154">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="5e88b-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="5e88b-155">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="5e88b-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="5e88b-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e88b-156">Example</span></span>
<span data-ttu-id="5e88b-157">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5e88b-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5e88b-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e88b-158">Request</span></span>
<span data-ttu-id="5e88b-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e88b-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="5e88b-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e88b-160">Response</span></span>
<span data-ttu-id="5e88b-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e88b-161">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-copytonotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
