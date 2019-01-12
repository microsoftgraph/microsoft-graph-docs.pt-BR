---
title: Atualizar orgcontact
description: Atualize as propriedades do objeto orgcontact.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f7943234dbff62da070b51a3ae6d92d2bdb28d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938815"
---
# <a name="update-orgcontact"></a><span data-ttu-id="c1ac3-103">Atualizar orgcontact</span><span class="sxs-lookup"><span data-stu-id="c1ac3-103">Update orgcontact</span></span>

> <span data-ttu-id="c1ac3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1ac3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1ac3-106">Atualize as propriedades do objeto orgcontact.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-106">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1ac3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1ac3-107">Permissions</span></span>
<span data-ttu-id="c1ac3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1ac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1ac3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1ac3-110">Permission type</span></span>      | <span data-ttu-id="c1ac3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1ac3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1ac3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-113">Not supported.</span></span>    |
|<span data-ttu-id="c1ac3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1ac3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1ac3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-115">Not supported.</span></span>    |
|<span data-ttu-id="c1ac3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1ac3-116">Application</span></span> | <span data-ttu-id="c1ac3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1ac3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1ac3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c1ac3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ac3-119">Request headers</span></span>
| <span data-ttu-id="c1ac3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c1ac3-120">Name</span></span>       | <span data-ttu-id="c1ac3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1ac3-121">Type</span></span> | <span data-ttu-id="c1ac3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1ac3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c1ac3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1ac3-123">Authorization</span></span>  | <span data-ttu-id="c1ac3-124">string</span><span class="sxs-lookup"><span data-stu-id="c1ac3-124">string</span></span>  | <span data-ttu-id="c1ac3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1ac3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ac3-127">Request body</span></span>
<span data-ttu-id="c1ac3-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c1ac3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1ac3-131">Property</span></span>     | <span data-ttu-id="c1ac3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1ac3-132">Type</span></span>   |<span data-ttu-id="c1ac3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1ac3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1ac3-134">city</span><span class="sxs-lookup"><span data-stu-id="c1ac3-134">city</span></span>|<span data-ttu-id="c1ac3-135">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-135">String</span></span>||
|<span data-ttu-id="c1ac3-136">country</span><span class="sxs-lookup"><span data-stu-id="c1ac3-136">country</span></span>|<span data-ttu-id="c1ac3-137">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-137">String</span></span>||
|<span data-ttu-id="c1ac3-138">departamento</span><span class="sxs-lookup"><span data-stu-id="c1ac3-138">department</span></span>|<span data-ttu-id="c1ac3-139">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-139">String</span></span>||
|<span data-ttu-id="c1ac3-140">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="c1ac3-140">onPremisesSyncEnabled</span></span>|<span data-ttu-id="c1ac3-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="c1ac3-141">Boolean</span></span>||
|<span data-ttu-id="c1ac3-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c1ac3-142">displayName</span></span>|<span data-ttu-id="c1ac3-143">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-143">String</span></span>||
|<span data-ttu-id="c1ac3-144">givenName</span><span class="sxs-lookup"><span data-stu-id="c1ac3-144">givenName</span></span>|<span data-ttu-id="c1ac3-145">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-145">String</span></span>||
|<span data-ttu-id="c1ac3-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="c1ac3-146">jobTitle</span></span>|<span data-ttu-id="c1ac3-147">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-147">String</span></span>||
|<span data-ttu-id="c1ac3-148">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ac3-148">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="c1ac3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ac3-149">DateTimeOffset</span></span>||
|<span data-ttu-id="c1ac3-150">Email</span><span class="sxs-lookup"><span data-stu-id="c1ac3-150">mail</span></span>|<span data-ttu-id="c1ac3-151">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-151">String</span></span>||
|<span data-ttu-id="c1ac3-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c1ac3-152">mailNickname</span></span>|<span data-ttu-id="c1ac3-153">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-153">String</span></span>||
|<span data-ttu-id="c1ac3-154">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="c1ac3-154">mobilePhone</span></span>|<span data-ttu-id="c1ac3-155">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-155">String</span></span>||
|<span data-ttu-id="c1ac3-156">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c1ac3-156">officeLocation</span></span>|<span data-ttu-id="c1ac3-157">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-157">String</span></span>||
|<span data-ttu-id="c1ac3-158">postalCode</span><span class="sxs-lookup"><span data-stu-id="c1ac3-158">postalCode</span></span>|<span data-ttu-id="c1ac3-159">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-159">String</span></span>||
|<span data-ttu-id="c1ac3-160">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="c1ac3-160">proxyAddresses</span></span>|<span data-ttu-id="c1ac3-161">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-161">String</span></span>||
|<span data-ttu-id="c1ac3-162">state</span><span class="sxs-lookup"><span data-stu-id="c1ac3-162">state</span></span>|<span data-ttu-id="c1ac3-163">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-163">String</span></span>||
|<span data-ttu-id="c1ac3-164">streetAddress</span><span class="sxs-lookup"><span data-stu-id="c1ac3-164">streetAddress</span></span>|<span data-ttu-id="c1ac3-165">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-165">String</span></span>||
|<span data-ttu-id="c1ac3-166">surname</span><span class="sxs-lookup"><span data-stu-id="c1ac3-166">surname</span></span>|<span data-ttu-id="c1ac3-167">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-167">String</span></span>||
|<span data-ttu-id="c1ac3-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="c1ac3-168">businessPhones</span></span>|<span data-ttu-id="c1ac3-169">String</span><span class="sxs-lookup"><span data-stu-id="c1ac3-169">String</span></span>||

## <a name="response"></a><span data-ttu-id="c1ac3-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1ac3-170">Response</span></span>

<span data-ttu-id="c1ac3-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-171">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1ac3-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1ac3-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1ac3-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ac3-173">Request</span></span>
<span data-ttu-id="c1ac3-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="c1ac3-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1ac3-175">Response</span></span>
<span data-ttu-id="c1ac3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1ac3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
