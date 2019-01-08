---
title: Atualizar privilegedapproval
description: Atualize as propriedades do objeto privilegedapproval.
ms.openlocfilehash: b50f5fb5e50bc47c94b759ea1253c9c9117bfe5d
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748350"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="2992a-103">Atualizar privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="2992a-103">Update privilegedapproval</span></span>

> <span data-ttu-id="2992a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2992a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2992a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2992a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2992a-106">Atualize as propriedades do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="2992a-106">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2992a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2992a-107">Permissions</span></span>
<span data-ttu-id="2992a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2992a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2992a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2992a-110">Permission type</span></span>      | <span data-ttu-id="2992a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2992a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2992a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2992a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2992a-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2992a-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2992a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2992a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2992a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2992a-115">Not supported.</span></span>    |
|<span data-ttu-id="2992a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2992a-116">Application</span></span> | <span data-ttu-id="2992a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2992a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2992a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2992a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="2992a-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2992a-119">Optional request headers</span></span>
| <span data-ttu-id="2992a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2992a-120">Name</span></span>       | <span data-ttu-id="2992a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2992a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2992a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2992a-122">Authorization</span></span>  | <span data-ttu-id="2992a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2992a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2992a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2992a-125">Request body</span></span>
<span data-ttu-id="2992a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2992a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2992a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2992a-129">Property</span></span>     | <span data-ttu-id="2992a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2992a-130">Type</span></span>   |<span data-ttu-id="2992a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2992a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2992a-132">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="2992a-132">approvalDuration</span></span>|<span data-ttu-id="2992a-133">Duração</span><span class="sxs-lookup"><span data-stu-id="2992a-133">Duration</span></span>||
|<span data-ttu-id="2992a-134">approvalState</span><span class="sxs-lookup"><span data-stu-id="2992a-134">approvalState</span></span>|<span data-ttu-id="2992a-135">string</span><span class="sxs-lookup"><span data-stu-id="2992a-135">string</span></span>| <span data-ttu-id="2992a-136">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="2992a-136">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="2992a-137">approvalType</span><span class="sxs-lookup"><span data-stu-id="2992a-137">approvalType</span></span>|<span data-ttu-id="2992a-138">String</span><span class="sxs-lookup"><span data-stu-id="2992a-138">String</span></span>||
|<span data-ttu-id="2992a-139">approverReason</span><span class="sxs-lookup"><span data-stu-id="2992a-139">approverReason</span></span>|<span data-ttu-id="2992a-140">String</span><span class="sxs-lookup"><span data-stu-id="2992a-140">String</span></span>||
|<span data-ttu-id="2992a-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2992a-141">endDateTime</span></span>|<span data-ttu-id="2992a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2992a-142">DateTimeOffset</span></span>||
|<span data-ttu-id="2992a-143">requestorReason</span><span class="sxs-lookup"><span data-stu-id="2992a-143">requestorReason</span></span>|<span data-ttu-id="2992a-144">String</span><span class="sxs-lookup"><span data-stu-id="2992a-144">String</span></span>||
|<span data-ttu-id="2992a-145">roleId</span><span class="sxs-lookup"><span data-stu-id="2992a-145">roleId</span></span>|<span data-ttu-id="2992a-146">String</span><span class="sxs-lookup"><span data-stu-id="2992a-146">String</span></span>||
|<span data-ttu-id="2992a-147">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2992a-147">startDateTime</span></span>|<span data-ttu-id="2992a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2992a-148">DateTimeOffset</span></span>||
|<span data-ttu-id="2992a-149">userId</span><span class="sxs-lookup"><span data-stu-id="2992a-149">userId</span></span>|<span data-ttu-id="2992a-150">String</span><span class="sxs-lookup"><span data-stu-id="2992a-150">String</span></span>||

## <a name="response"></a><span data-ttu-id="2992a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2992a-151">Response</span></span>

<span data-ttu-id="2992a-152">Se tiver êxito, este método retornará um `204 No Content` código de resposta</span><span class="sxs-lookup"><span data-stu-id="2992a-152">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="2992a-153">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="2992a-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2992a-154">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="2992a-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="2992a-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2992a-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2992a-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2992a-156">Request</span></span>
<span data-ttu-id="2992a-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2992a-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval{request-id}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a><span data-ttu-id="2992a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="2992a-158">Response</span></span>
<span data-ttu-id="2992a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2992a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
