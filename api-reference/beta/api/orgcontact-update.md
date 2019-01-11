---
title: Atualizar orgcontact
description: Atualize as propriedades do objeto orgcontact.
localization_priority: Normal
ms.openlocfilehash: f48795bef6ea1a4833379f54747cbf2c291b2454
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859063"
---
# <a name="update-orgcontact"></a><span data-ttu-id="61663-103">Atualizar orgcontact</span><span class="sxs-lookup"><span data-stu-id="61663-103">Update orgcontact</span></span>

> <span data-ttu-id="61663-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61663-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61663-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61663-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61663-106">Atualize as propriedades do objeto orgcontact.</span><span class="sxs-lookup"><span data-stu-id="61663-106">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="61663-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="61663-107">Permissions</span></span>
<span data-ttu-id="61663-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61663-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61663-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61663-110">Permission type</span></span>      | <span data-ttu-id="61663-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61663-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61663-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61663-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61663-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61663-113">Not supported.</span></span>    |
|<span data-ttu-id="61663-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61663-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61663-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61663-115">Not supported.</span></span>    |
|<span data-ttu-id="61663-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61663-116">Application</span></span> | <span data-ttu-id="61663-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61663-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61663-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61663-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="61663-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61663-119">Request headers</span></span>
| <span data-ttu-id="61663-120">Nome</span><span class="sxs-lookup"><span data-stu-id="61663-120">Name</span></span>       | <span data-ttu-id="61663-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="61663-121">Type</span></span> | <span data-ttu-id="61663-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="61663-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="61663-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61663-123">Authorization</span></span>  | <span data-ttu-id="61663-124">string</span><span class="sxs-lookup"><span data-stu-id="61663-124">string</span></span>  | <span data-ttu-id="61663-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61663-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61663-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61663-127">Request body</span></span>
<span data-ttu-id="61663-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="61663-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="61663-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61663-131">Property</span></span>     | <span data-ttu-id="61663-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="61663-132">Type</span></span>   |<span data-ttu-id="61663-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="61663-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61663-134">city</span><span class="sxs-lookup"><span data-stu-id="61663-134">city</span></span>|<span data-ttu-id="61663-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-135">String</span></span>||
|<span data-ttu-id="61663-136">country</span><span class="sxs-lookup"><span data-stu-id="61663-136">country</span></span>|<span data-ttu-id="61663-137">String</span><span class="sxs-lookup"><span data-stu-id="61663-137">String</span></span>||
|<span data-ttu-id="61663-138">departamento</span><span class="sxs-lookup"><span data-stu-id="61663-138">department</span></span>|<span data-ttu-id="61663-139">String</span><span class="sxs-lookup"><span data-stu-id="61663-139">String</span></span>||
|<span data-ttu-id="61663-140">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="61663-140">onPremisesSyncEnabled</span></span>|<span data-ttu-id="61663-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="61663-141">Boolean</span></span>||
|<span data-ttu-id="61663-142">displayName</span><span class="sxs-lookup"><span data-stu-id="61663-142">displayName</span></span>|<span data-ttu-id="61663-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-143">String</span></span>||
|<span data-ttu-id="61663-144">givenName</span><span class="sxs-lookup"><span data-stu-id="61663-144">givenName</span></span>|<span data-ttu-id="61663-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-145">String</span></span>||
|<span data-ttu-id="61663-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="61663-146">jobTitle</span></span>|<span data-ttu-id="61663-147">String</span><span class="sxs-lookup"><span data-stu-id="61663-147">String</span></span>||
|<span data-ttu-id="61663-148">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="61663-148">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="61663-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61663-149">DateTimeOffset</span></span>||
|<span data-ttu-id="61663-150">Email</span><span class="sxs-lookup"><span data-stu-id="61663-150">mail</span></span>|<span data-ttu-id="61663-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-151">String</span></span>||
|<span data-ttu-id="61663-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="61663-152">mailNickname</span></span>|<span data-ttu-id="61663-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-153">String</span></span>||
|<span data-ttu-id="61663-154">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="61663-154">mobilePhone</span></span>|<span data-ttu-id="61663-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-155">String</span></span>||
|<span data-ttu-id="61663-156">officeLocation</span><span class="sxs-lookup"><span data-stu-id="61663-156">officeLocation</span></span>|<span data-ttu-id="61663-157">String</span><span class="sxs-lookup"><span data-stu-id="61663-157">String</span></span>||
|<span data-ttu-id="61663-158">postalCode</span><span class="sxs-lookup"><span data-stu-id="61663-158">postalCode</span></span>|<span data-ttu-id="61663-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-159">String</span></span>||
|<span data-ttu-id="61663-160">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="61663-160">proxyAddresses</span></span>|<span data-ttu-id="61663-161">String</span><span class="sxs-lookup"><span data-stu-id="61663-161">String</span></span>||
|<span data-ttu-id="61663-162">state</span><span class="sxs-lookup"><span data-stu-id="61663-162">state</span></span>|<span data-ttu-id="61663-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-163">String</span></span>||
|<span data-ttu-id="61663-164">streetAddress</span><span class="sxs-lookup"><span data-stu-id="61663-164">streetAddress</span></span>|<span data-ttu-id="61663-165">String</span><span class="sxs-lookup"><span data-stu-id="61663-165">String</span></span>||
|<span data-ttu-id="61663-166">surname</span><span class="sxs-lookup"><span data-stu-id="61663-166">surname</span></span>|<span data-ttu-id="61663-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61663-167">String</span></span>||
|<span data-ttu-id="61663-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="61663-168">businessPhones</span></span>|<span data-ttu-id="61663-169">String</span><span class="sxs-lookup"><span data-stu-id="61663-169">String</span></span>||

## <a name="response"></a><span data-ttu-id="61663-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="61663-170">Response</span></span>

<span data-ttu-id="61663-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61663-171">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61663-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61663-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61663-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61663-173">Request</span></span>
<span data-ttu-id="61663-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61663-174">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="61663-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="61663-175">Response</span></span>
<span data-ttu-id="61663-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61663-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
