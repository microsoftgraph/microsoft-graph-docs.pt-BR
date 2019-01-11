---
title: 'section: copyToSectionGroup'
description: Copia uma seção para um grupo de seção específico.
localization_priority: Normal
ms.openlocfilehash: 671cd28db66517b0b04d8b9d99cc1dccba17206e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846568"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="4225b-103">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="4225b-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="4225b-104">Copia uma seção para um grupo de seção específico.</span><span class="sxs-lookup"><span data-stu-id="4225b-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="4225b-105">Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e sonde o ponto de extremidade da operação para ver o resultado.</span><span class="sxs-lookup"><span data-stu-id="4225b-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="4225b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4225b-106">Permissions</span></span>
<span data-ttu-id="4225b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4225b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4225b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4225b-109">Permission type</span></span>      | <span data-ttu-id="4225b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4225b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4225b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4225b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4225b-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4225b-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4225b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4225b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4225b-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4225b-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4225b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4225b-115">Application</span></span> | <span data-ttu-id="4225b-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4225b-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4225b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4225b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="4225b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4225b-118">Request headers</span></span>
| <span data-ttu-id="4225b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4225b-119">Name</span></span>       | <span data-ttu-id="4225b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4225b-120">Type</span></span> | <span data-ttu-id="4225b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4225b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4225b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4225b-122">Authorization</span></span>  | <span data-ttu-id="4225b-123">string</span><span class="sxs-lookup"><span data-stu-id="4225b-123">string</span></span>  | <span data-ttu-id="4225b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4225b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4225b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4225b-126">Content-Type</span></span> | <span data-ttu-id="4225b-127">string</span><span class="sxs-lookup"><span data-stu-id="4225b-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4225b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4225b-128">Request body</span></span>
<span data-ttu-id="4225b-129">No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.</span><span class="sxs-lookup"><span data-stu-id="4225b-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="4225b-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4225b-130">Parameter</span></span>    | <span data-ttu-id="4225b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4225b-131">Type</span></span>   |<span data-ttu-id="4225b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4225b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4225b-133">groupId</span><span class="sxs-lookup"><span data-stu-id="4225b-133">groupId</span></span>|<span data-ttu-id="4225b-134">String</span><span class="sxs-lookup"><span data-stu-id="4225b-134">String</span></span>|<span data-ttu-id="4225b-p103">A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4225b-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="4225b-137">id</span><span class="sxs-lookup"><span data-stu-id="4225b-137">id</span></span>|<span data-ttu-id="4225b-138">String</span><span class="sxs-lookup"><span data-stu-id="4225b-138">String</span></span>|<span data-ttu-id="4225b-p104">Obrigatório. A id do grupo de seção de destino.</span><span class="sxs-lookup"><span data-stu-id="4225b-p104">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="4225b-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="4225b-141">renameAs</span></span>|<span data-ttu-id="4225b-142">String</span><span class="sxs-lookup"><span data-stu-id="4225b-142">String</span></span>|<span data-ttu-id="4225b-p105">O nome da cópia. Restabelece o padrão do nome do item existente.</span><span class="sxs-lookup"><span data-stu-id="4225b-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="4225b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4225b-145">Response</span></span>

<span data-ttu-id="4225b-p106">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="4225b-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4225b-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4225b-148">Example</span></span>
<span data-ttu-id="4225b-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4225b-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4225b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4225b-150">Request</span></span>
<span data-ttu-id="4225b-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4225b-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="4225b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="4225b-152">Response</span></span>
<span data-ttu-id="4225b-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4225b-153">Here is an example of the response.</span></span>
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
