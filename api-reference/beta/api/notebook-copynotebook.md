---
title: 'bloco de anotações: copyNotebook'
description: Copia um bloco de anotações para a pasta blocos de anotações na biblioteca de documentos de destino. A pasta é criada se não existir.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 693268bc8f9343e93a2edeece4e232cfc15224fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333117"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="9a886-104">bloco de anotações: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="9a886-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a886-105">Copia um bloco de anotações para a pasta blocos de anotações na biblioteca de documentos de destino.</span><span class="sxs-lookup"><span data-stu-id="9a886-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="9a886-106">A pasta é criada se não existir.</span><span class="sxs-lookup"><span data-stu-id="9a886-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="9a886-107">Para operações de cópia, siga um padrão de chamada assíncrona: primeiro, chame a ação de cópia e, em seguida, pesquise o ponto de extremidade da operação para o resultado.</span><span class="sxs-lookup"><span data-stu-id="9a886-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a886-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a886-108">Permissions</span></span>
<span data-ttu-id="9a886-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a886-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a886-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a886-111">Permission type</span></span>      | <span data-ttu-id="9a886-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a886-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a886-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a886-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9a886-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a886-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a886-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a886-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a886-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a886-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9a886-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a886-117">Application</span></span> | <span data-ttu-id="9a886-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a886-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a886-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a886-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="9a886-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a886-120">Request headers</span></span>
| <span data-ttu-id="9a886-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9a886-121">Name</span></span>       | <span data-ttu-id="9a886-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a886-122">Type</span></span> | <span data-ttu-id="9a886-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a886-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a886-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a886-124">Authorization</span></span>  | <span data-ttu-id="9a886-125">string</span><span class="sxs-lookup"><span data-stu-id="9a886-125">string</span></span>  | <span data-ttu-id="9a886-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a886-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a886-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a886-128">Content-Type</span></span> | <span data-ttu-id="9a886-129">string</span><span class="sxs-lookup"><span data-stu-id="9a886-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9a886-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a886-130">Request body</span></span>
<span data-ttu-id="9a886-131">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros de que sua operação precisa.</span><span class="sxs-lookup"><span data-stu-id="9a886-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="9a886-132">É possível enviar um corpo vazio se nenhum for necessário.</span><span class="sxs-lookup"><span data-stu-id="9a886-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="9a886-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9a886-133">Parameter</span></span>    | <span data-ttu-id="9a886-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a886-134">Type</span></span>   |<span data-ttu-id="9a886-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a886-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a886-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="9a886-136">siteCollectionId</span></span>|<span data-ttu-id="9a886-137">String</span><span class="sxs-lookup"><span data-stu-id="9a886-137">String</span></span>|<span data-ttu-id="9a886-138">A ID do site do SharePoint para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="9a886-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="9a886-139">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9a886-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="9a886-140">siteId</span><span class="sxs-lookup"><span data-stu-id="9a886-140">siteId</span></span>|<span data-ttu-id="9a886-141">String</span><span class="sxs-lookup"><span data-stu-id="9a886-141">String</span></span>|<span data-ttu-id="9a886-142">A ID da Web do SharePoint a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="9a886-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="9a886-143">Use somente ao copiar para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9a886-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="9a886-144">groupId</span><span class="sxs-lookup"><span data-stu-id="9a886-144">groupId</span></span>|<span data-ttu-id="9a886-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a886-145">String</span></span>|<span data-ttu-id="9a886-146">A ID do grupo para o qual copiar.</span><span class="sxs-lookup"><span data-stu-id="9a886-146">The id of the group to copy to.</span></span> <span data-ttu-id="9a886-147">Use somente ao copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9a886-147">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="9a886-148">renomeas</span><span class="sxs-lookup"><span data-stu-id="9a886-148">renameAs</span></span>|<span data-ttu-id="9a886-149">String</span><span class="sxs-lookup"><span data-stu-id="9a886-149">String</span></span>|<span data-ttu-id="9a886-150">O nome da cópia.</span><span class="sxs-lookup"><span data-stu-id="9a886-150">The name of the copy.</span></span> <span data-ttu-id="9a886-151">O padrão é o nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="9a886-151">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="9a886-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a886-152">Response</span></span>

<span data-ttu-id="9a886-153">Se tiver êxito, este método retornará `202 Accepted` um código de resposta `Operation-Location` e um cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="9a886-153">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="9a886-154">Sondar o ponto de extremidade da operação-local para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="9a886-154">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="9a886-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a886-155">Example</span></span>
<span data-ttu-id="9a886-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9a886-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a886-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a886-157">Request</span></span>
<span data-ttu-id="9a886-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a886-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="9a886-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a886-159">Response</span></span>
<span data-ttu-id="9a886-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a886-160">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
