---
title: 'notebook: copyNotebook'
description: Copia um bloco de anotações para a pasta Blocos de anotações na biblioteca de documentos de destino. Se a pasta não existir, ela será criada.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7100d768fb411aeab8ccbd0622de26aeae8a7133
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515598"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="b0bec-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="b0bec-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0bec-p102">Copia um bloco de anotações para a pasta Blocos de anotações na biblioteca de documentos de destino. Se a pasta não existir, ela será criada.</span><span class="sxs-lookup"><span data-stu-id="b0bec-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="b0bec-107">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="b0bec-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0bec-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0bec-108">Permissions</span></span>
<span data-ttu-id="b0bec-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0bec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0bec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0bec-111">Permission type</span></span>      | <span data-ttu-id="b0bec-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0bec-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0bec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0bec-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b0bec-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0bec-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0bec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0bec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0bec-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0bec-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b0bec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0bec-117">Application</span></span> | <span data-ttu-id="b0bec-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0bec-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0bec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0bec-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="b0bec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0bec-120">Request headers</span></span>
| <span data-ttu-id="b0bec-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b0bec-121">Name</span></span>       | <span data-ttu-id="b0bec-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0bec-122">Type</span></span> | <span data-ttu-id="b0bec-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0bec-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b0bec-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0bec-124">Authorization</span></span>  | <span data-ttu-id="b0bec-125">string</span><span class="sxs-lookup"><span data-stu-id="b0bec-125">string</span></span>  | <span data-ttu-id="b0bec-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0bec-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0bec-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0bec-128">Content-Type</span></span> | <span data-ttu-id="b0bec-129">string</span><span class="sxs-lookup"><span data-stu-id="b0bec-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b0bec-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0bec-130">Request body</span></span>
<span data-ttu-id="b0bec-p105">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa. É possível enviar um corpo vazio se nenhum objeto for necessário.</span><span class="sxs-lookup"><span data-stu-id="b0bec-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="b0bec-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b0bec-133">Parameter</span></span>    | <span data-ttu-id="b0bec-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0bec-134">Type</span></span>   |<span data-ttu-id="b0bec-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0bec-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0bec-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="b0bec-136">siteCollectionId</span></span>|<span data-ttu-id="b0bec-137">String</span><span class="sxs-lookup"><span data-stu-id="b0bec-137">String</span></span>|<span data-ttu-id="b0bec-138">A identificação do site do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="b0bec-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="b0bec-139">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b0bec-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b0bec-140">siteId</span><span class="sxs-lookup"><span data-stu-id="b0bec-140">siteId</span></span>|<span data-ttu-id="b0bec-141">String</span><span class="sxs-lookup"><span data-stu-id="b0bec-141">String</span></span>|<span data-ttu-id="b0bec-142">A identificação da web do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="b0bec-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="b0bec-143">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b0bec-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b0bec-144">groupId</span><span class="sxs-lookup"><span data-stu-id="b0bec-144">groupId</span></span>|<span data-ttu-id="b0bec-145">String</span><span class="sxs-lookup"><span data-stu-id="b0bec-145">String</span></span>|<span data-ttu-id="b0bec-p108">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b0bec-p108">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="b0bec-148">renameAs</span><span class="sxs-lookup"><span data-stu-id="b0bec-148">renameAs</span></span>|<span data-ttu-id="b0bec-149">String</span><span class="sxs-lookup"><span data-stu-id="b0bec-149">String</span></span>|<span data-ttu-id="b0bec-p109">O nome da cópia. Restabelece o padrão do nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="b0bec-p109">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="b0bec-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0bec-152">Response</span></span>

<span data-ttu-id="b0bec-p110">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="b0bec-p110">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b0bec-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0bec-155">Example</span></span>
<span data-ttu-id="b0bec-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b0bec-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b0bec-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0bec-157">Request</span></span>
<span data-ttu-id="b0bec-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0bec-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b0bec-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0bec-159">Response</span></span>
<span data-ttu-id="b0bec-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0bec-160">Here is an example of the response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-copynotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
