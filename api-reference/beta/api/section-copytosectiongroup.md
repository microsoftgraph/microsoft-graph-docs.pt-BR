---
title: 'section: copyToSectionGroup'
description: Copia uma seção para um grupo de seção específico.
ms.openlocfilehash: c73f24084c26d8b4c715ab164267bbc41c74ceb3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035653"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="607db-103">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="607db-103">section: copyToSectionGroup</span></span>

> <span data-ttu-id="607db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="607db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="607db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="607db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="607db-106">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="607db-106">Copies a section to a specific section group.</span></span>

<span data-ttu-id="607db-107">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="607db-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="607db-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="607db-108">Permissions</span></span>
<span data-ttu-id="607db-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="607db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="607db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="607db-111">Permission type</span></span>      | <span data-ttu-id="607db-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="607db-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="607db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="607db-113">Delegated (work or school account)</span></span> | <span data-ttu-id="607db-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607db-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="607db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="607db-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="607db-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="607db-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="607db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="607db-117">Application</span></span> | <span data-ttu-id="607db-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607db-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="607db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="607db-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="607db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="607db-120">Request headers</span></span>
| <span data-ttu-id="607db-121">Nome</span><span class="sxs-lookup"><span data-stu-id="607db-121">Name</span></span>       | <span data-ttu-id="607db-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="607db-122">Type</span></span> | <span data-ttu-id="607db-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="607db-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="607db-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="607db-124">Authorization</span></span>  | <span data-ttu-id="607db-125">string</span><span class="sxs-lookup"><span data-stu-id="607db-125">string</span></span>  | <span data-ttu-id="607db-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="607db-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="607db-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="607db-128">Content-Type</span></span> | <span data-ttu-id="607db-129">string</span><span class="sxs-lookup"><span data-stu-id="607db-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="607db-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="607db-130">Request body</span></span>
<span data-ttu-id="607db-131">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.</span><span class="sxs-lookup"><span data-stu-id="607db-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="607db-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="607db-132">Parameter</span></span>    | <span data-ttu-id="607db-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="607db-133">Type</span></span>   |<span data-ttu-id="607db-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="607db-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="607db-135">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="607db-135">siteCollectionId</span></span>|<span data-ttu-id="607db-136">String</span><span class="sxs-lookup"><span data-stu-id="607db-136">String</span></span>|<span data-ttu-id="607db-137">A identificação do site do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="607db-137">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="607db-138">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="607db-138">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="607db-139">siteId</span><span class="sxs-lookup"><span data-stu-id="607db-139">siteId</span></span>|<span data-ttu-id="607db-140">String</span><span class="sxs-lookup"><span data-stu-id="607db-140">String</span></span>|<span data-ttu-id="607db-141">A identificação da web do SharePoint para copiar.</span><span class="sxs-lookup"><span data-stu-id="607db-141">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="607db-142">Use somente quando a cópia para um site de equipe do Office 365.</span><span class="sxs-lookup"><span data-stu-id="607db-142">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="607db-143">groupId</span><span class="sxs-lookup"><span data-stu-id="607db-143">groupId</span></span>|<span data-ttu-id="607db-144">String</span><span class="sxs-lookup"><span data-stu-id="607db-144">String</span></span>|<span data-ttu-id="607db-p106">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="607db-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="607db-147">id</span><span class="sxs-lookup"><span data-stu-id="607db-147">id</span></span>|<span data-ttu-id="607db-148">String</span><span class="sxs-lookup"><span data-stu-id="607db-148">String</span></span>|<span data-ttu-id="607db-p107">Obrigatório. A id do grupo de seção de destino.</span><span class="sxs-lookup"><span data-stu-id="607db-p107">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="607db-151">renameAs</span><span class="sxs-lookup"><span data-stu-id="607db-151">renameAs</span></span>|<span data-ttu-id="607db-152">String</span><span class="sxs-lookup"><span data-stu-id="607db-152">String</span></span>|<span data-ttu-id="607db-p108">O nome da cópia. Restabelece o padrão do nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="607db-p108">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="607db-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="607db-155">Response</span></span>

<span data-ttu-id="607db-p109">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="607db-p109">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="607db-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="607db-158">Example</span></span>
<span data-ttu-id="607db-159">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="607db-159">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="607db-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="607db-160">Request</span></span>
<span data-ttu-id="607db-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="607db-161">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="607db-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="607db-162">Response</span></span>
<span data-ttu-id="607db-163">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="607db-163">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->