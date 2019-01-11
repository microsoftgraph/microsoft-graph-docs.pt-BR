---
title: 'notebook: copyNotebook'
description: Copia um bloco de anotações para a pasta Blocos de anotações na biblioteca de documentos de destino. Se a pasta não existir, ela será criada.
localization_priority: Normal
ms.openlocfilehash: ba9ed886ab0102a3ed66c31efbc420832e67d316
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833051"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="45ca0-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="45ca0-104">notebook: copyNotebook</span></span>

> <span data-ttu-id="45ca0-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="45ca0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45ca0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45ca0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45ca0-p103">Copia um bloco de anotações para a pasta Blocos de anotações na biblioteca de documentos de destino. Se a pasta não existir, ela será criada.</span><span class="sxs-lookup"><span data-stu-id="45ca0-p103">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="45ca0-109">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="45ca0-109">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="45ca0-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="45ca0-110">Permissions</span></span>
<span data-ttu-id="45ca0-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45ca0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45ca0-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45ca0-113">Permission type</span></span>      | <span data-ttu-id="45ca0-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45ca0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45ca0-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45ca0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="45ca0-116">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45ca0-116">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="45ca0-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45ca0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45ca0-118">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45ca0-118">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="45ca0-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45ca0-119">Application</span></span> | <span data-ttu-id="45ca0-120">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45ca0-120">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45ca0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45ca0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="45ca0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45ca0-122">Request headers</span></span>
| <span data-ttu-id="45ca0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="45ca0-123">Name</span></span>       | <span data-ttu-id="45ca0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="45ca0-124">Type</span></span> | <span data-ttu-id="45ca0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="45ca0-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="45ca0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="45ca0-126">Authorization</span></span>  | <span data-ttu-id="45ca0-127">string</span><span class="sxs-lookup"><span data-stu-id="45ca0-127">string</span></span>  | <span data-ttu-id="45ca0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45ca0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45ca0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45ca0-130">Content-Type</span></span> | <span data-ttu-id="45ca0-131">string</span><span class="sxs-lookup"><span data-stu-id="45ca0-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="45ca0-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45ca0-132">Request body</span></span>
<span data-ttu-id="45ca0-p106">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa. É possível enviar um corpo vazio se nenhum objeto for necessário.</span><span class="sxs-lookup"><span data-stu-id="45ca0-p106">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="45ca0-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="45ca0-135">Parameter</span></span>    | <span data-ttu-id="45ca0-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="45ca0-136">Type</span></span>   |<span data-ttu-id="45ca0-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="45ca0-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45ca0-138">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="45ca0-138">siteCollectionId</span></span>|<span data-ttu-id="45ca0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45ca0-139">String</span></span>|<span data-ttu-id="45ca0-140">A identificação do site do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="45ca0-140">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="45ca0-141">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="45ca0-141">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="45ca0-142">siteId</span><span class="sxs-lookup"><span data-stu-id="45ca0-142">siteId</span></span>|<span data-ttu-id="45ca0-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45ca0-143">String</span></span>|<span data-ttu-id="45ca0-144">A identificação da web do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="45ca0-144">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="45ca0-145">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="45ca0-145">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="45ca0-146">groupId</span><span class="sxs-lookup"><span data-stu-id="45ca0-146">groupId</span></span>|<span data-ttu-id="45ca0-147">String</span><span class="sxs-lookup"><span data-stu-id="45ca0-147">String</span></span>|<span data-ttu-id="45ca0-p109">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="45ca0-p109">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="45ca0-150">renameAs</span><span class="sxs-lookup"><span data-stu-id="45ca0-150">renameAs</span></span>|<span data-ttu-id="45ca0-151">String</span><span class="sxs-lookup"><span data-stu-id="45ca0-151">String</span></span>|<span data-ttu-id="45ca0-p110">O nome da cópia. Restabelece o padrão do nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="45ca0-p110">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="45ca0-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="45ca0-154">Response</span></span>

<span data-ttu-id="45ca0-p111">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="45ca0-p111">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="45ca0-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45ca0-157">Example</span></span>
<span data-ttu-id="45ca0-158">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="45ca0-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="45ca0-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45ca0-159">Request</span></span>
<span data-ttu-id="45ca0-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45ca0-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="45ca0-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="45ca0-161">Response</span></span>
<span data-ttu-id="45ca0-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45ca0-162">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
