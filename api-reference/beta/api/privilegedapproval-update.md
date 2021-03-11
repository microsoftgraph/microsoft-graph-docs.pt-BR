---
title: Atualizar privilegedapproval
description: Atualize as propriedades do objeto privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a04f33c283cd82715cb1e0d63917cea7cb373329
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720456"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="5e902-103">Atualizar privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="5e902-103">Update privilegedapproval</span></span>

<span data-ttu-id="5e902-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e902-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e902-105">Atualize as propriedades do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="5e902-105">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e902-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e902-106">Permissions</span></span>
<span data-ttu-id="5e902-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5e902-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e902-109">Permission type</span></span>      | <span data-ttu-id="5e902-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e902-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e902-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e902-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e902-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5e902-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e902-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e902-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e902-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e902-114">Not supported.</span></span>    |
|<span data-ttu-id="5e902-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e902-115">Application</span></span> | <span data-ttu-id="5e902-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e902-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e902-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e902-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5e902-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5e902-118">Optional request headers</span></span>
| <span data-ttu-id="5e902-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5e902-119">Name</span></span>       | <span data-ttu-id="5e902-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e902-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5e902-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e902-121">Authorization</span></span>  | <span data-ttu-id="5e902-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e902-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e902-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e902-124">Request body</span></span>
<span data-ttu-id="5e902-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5e902-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e902-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e902-128">Property</span></span>     | <span data-ttu-id="5e902-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e902-129">Type</span></span>   |<span data-ttu-id="5e902-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e902-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e902-131">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="5e902-131">approvalDuration</span></span>|<span data-ttu-id="5e902-132">Duration</span><span class="sxs-lookup"><span data-stu-id="5e902-132">Duration</span></span>||
|<span data-ttu-id="5e902-133">approvalState</span><span class="sxs-lookup"><span data-stu-id="5e902-133">approvalState</span></span>|<span data-ttu-id="5e902-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e902-134">string</span></span>| <span data-ttu-id="5e902-135">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="5e902-135">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="5e902-136">approvalType</span><span class="sxs-lookup"><span data-stu-id="5e902-136">approvalType</span></span>|<span data-ttu-id="5e902-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e902-137">String</span></span>||
|<span data-ttu-id="5e902-138">approverReason</span><span class="sxs-lookup"><span data-stu-id="5e902-138">approverReason</span></span>|<span data-ttu-id="5e902-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e902-139">String</span></span>||
|<span data-ttu-id="5e902-140">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5e902-140">endDateTime</span></span>|<span data-ttu-id="5e902-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e902-141">DateTimeOffset</span></span>||
|<span data-ttu-id="5e902-142">requestorReason</span><span class="sxs-lookup"><span data-stu-id="5e902-142">requestorReason</span></span>|<span data-ttu-id="5e902-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e902-143">String</span></span>||
|<span data-ttu-id="5e902-144">roleId</span><span class="sxs-lookup"><span data-stu-id="5e902-144">roleId</span></span>|<span data-ttu-id="5e902-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e902-145">String</span></span>||
|<span data-ttu-id="5e902-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5e902-146">startDateTime</span></span>|<span data-ttu-id="5e902-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e902-147">DateTimeOffset</span></span>||
|<span data-ttu-id="5e902-148">userId</span><span class="sxs-lookup"><span data-stu-id="5e902-148">userId</span></span>|<span data-ttu-id="5e902-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e902-149">String</span></span>||

## <a name="response"></a><span data-ttu-id="5e902-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e902-150">Response</span></span>

<span data-ttu-id="5e902-151">Se tiver êxito, este método retornará um `204 No Content` código de resposta</span><span class="sxs-lookup"><span data-stu-id="5e902-151">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="5e902-152">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="5e902-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5e902-153">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="5e902-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="5e902-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e902-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e902-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e902-155">Request</span></span>
<span data-ttu-id="5e902-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e902-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval/{requestId}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a><span data-ttu-id="5e902-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e902-157">Response</span></span>
<span data-ttu-id="5e902-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e902-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


