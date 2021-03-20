---
title: Atualizar secureScoreControlProfile
description: Atualize um objeto secureScoreControlProfile editável em qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: ddedbb28f16defa68cecd9d03ac24174c916b175
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948756"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="b645b-103">Atualizar secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="b645b-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="b645b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b645b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b645b-105">Atualizar um objeto **secureScoreControlProfile** editável em qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="b645b-105">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="b645b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b645b-106">Permissions</span></span>

<span data-ttu-id="b645b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b645b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b645b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b645b-109">Permission type</span></span>      | <span data-ttu-id="b645b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b645b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b645b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b645b-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="b645b-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b645b-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="b645b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b645b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b645b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b645b-114">Not supported.</span></span>  |
|<span data-ttu-id="b645b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b645b-115">Application</span></span> | <span data-ttu-id="b645b-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b645b-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b645b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b645b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b645b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b645b-118">Request headers</span></span>

| <span data-ttu-id="b645b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b645b-119">Name</span></span>       | <span data-ttu-id="b645b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b645b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b645b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b645b-121">Authorization</span></span>  | <span data-ttu-id="b645b-122">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="b645b-122">Bearer {code}.</span></span> <span data-ttu-id="b645b-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b645b-123">Required.</span></span>|
|<span data-ttu-id="b645b-124">Preferir</span><span class="sxs-lookup"><span data-stu-id="b645b-124">Prefer</span></span> | <span data-ttu-id="b645b-125">return=representation.</span><span class="sxs-lookup"><span data-stu-id="b645b-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b645b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b645b-126">Request body</span></span>

<span data-ttu-id="b645b-127">No corpo da solicitação, fornece uma representação JSON dos valores para campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b645b-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b645b-128">O corpo **deve** conter a `vendorInformation` propriedade com campos `provider` `vendor` válidos e válidos.</span><span class="sxs-lookup"><span data-stu-id="b645b-128">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="b645b-129">A tabela a seguir lista os campos que podem ser atualizados para **um secureScoreControlProfile**.</span><span class="sxs-lookup"><span data-stu-id="b645b-129">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="b645b-130">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="b645b-130">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="b645b-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b645b-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b645b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b645b-132">Property</span></span>   | <span data-ttu-id="b645b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b645b-133">Type</span></span> |<span data-ttu-id="b645b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b645b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b645b-135">assignedTo</span><span class="sxs-lookup"><span data-stu-id="b645b-135">assignedTo</span></span>|<span data-ttu-id="b645b-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b645b-136">String</span></span>|<span data-ttu-id="b645b-137">Nome do analista ao que o controle é atribuído para triagem, implementação ou correção.</span><span class="sxs-lookup"><span data-stu-id="b645b-137">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="b645b-138">comment</span><span class="sxs-lookup"><span data-stu-id="b645b-138">comment</span></span>|<span data-ttu-id="b645b-139">String</span><span class="sxs-lookup"><span data-stu-id="b645b-139">String</span></span>|<span data-ttu-id="b645b-140">Comentários do analista sobre o controle (para gerenciamento de controle do cliente).</span><span class="sxs-lookup"><span data-stu-id="b645b-140">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="b645b-141">estado</span><span class="sxs-lookup"><span data-stu-id="b645b-141">state</span></span>| <span data-ttu-id="b645b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b645b-142">String</span></span>|<span data-ttu-id="b645b-143">Configuração orientada pelo analista no controle.</span><span class="sxs-lookup"><span data-stu-id="b645b-143">Analyst driven setting on the control.</span></span> <span data-ttu-id="b645b-144">Os valores possíveis são: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span><span class="sxs-lookup"><span data-stu-id="b645b-144">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="b645b-145">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="b645b-145">vendorInformation</span></span> | [<span data-ttu-id="b645b-146">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="b645b-146">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="b645b-147">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, provedor e subprovider (por exemplo, vendor=Microsoft; provider=SecureScore;).</span><span class="sxs-lookup"><span data-stu-id="b645b-147">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="b645b-148">**Os campos provedor e fornecedor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="b645b-148">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="b645b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b645b-149">Response</span></span>

<span data-ttu-id="b645b-150">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b645b-150">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="b645b-151">Se o header de solicitação opcional for usado, o método retornará um código de resposta e o objeto `200 OK` [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b645b-151">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b645b-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b645b-152">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="b645b-153">Exemplo 1: Solicitar sem o header Prefer</span><span class="sxs-lookup"><span data-stu-id="b645b-153">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="b645b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b645b-154">Request</span></span>

<span data-ttu-id="b645b-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b645b-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b645b-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="b645b-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update_1"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {

    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="b645b-157">C#</span><span class="sxs-lookup"><span data-stu-id="b645b-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b645b-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b645b-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b645b-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b645b-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b645b-160">Java</span><span class="sxs-lookup"><span data-stu-id="b645b-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b645b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b645b-161">Response</span></span>

<span data-ttu-id="b645b-162">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="b645b-162">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="b645b-163">Exemplo 2: Solicitar com o header Prefer</span><span class="sxs-lookup"><span data-stu-id="b645b-163">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="b645b-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b645b-164">Request</span></span>

<span data-ttu-id="b645b-165">O exemplo a seguir mostra uma solicitação que inclui o `Prefer` header de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b645b-165">The following example shows a request that includes the `Prefer` request header.</span></span>


# <a name="http"></a>[<span data-ttu-id="b645b-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="b645b-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update_2"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="b645b-167">C#</span><span class="sxs-lookup"><span data-stu-id="b645b-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b645b-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b645b-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b645b-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b645b-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b645b-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="b645b-170">Response</span></span>

<span data-ttu-id="b645b-171">A seguir, um exemplo da resposta quando o `Prefer: return=representation` header de solicitação opcional é usado.</span><span class="sxs-lookup"><span data-stu-id="b645b-171">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="b645b-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b645b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "NonOwnerAccess",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Review",
  "actionUrl": "https://outlook.office365.com/NonOwnerAccessReport.aspx",
  "controlCategory": "Data",
  "title": "Review mailbox access by non-owners bi-weekly", 
  "deprecated": false,
  "implementationCost": "Low",
  "lastModifiedDateTime": null,
  "maxScore": 5.0,
  "rank": 25,
  "remediation": "Once you have opened the search tool, specify a date range and select access by <b>All non-owners</b> or <b>External users</b>",
  "remediationImpact": "This change will have no effect on your users",
  "service": "EXO",
  "threats": [
    "Account Breach",
    "Data Exfiltration",
    "Malicious Insider"
  ],
  "tier": "Core",
  "userImpact": "Low",
  "complianceInformation": [
    {
      "certificationName": "FedRAMP_Moderate",
      "certificationControls": [
        {
          "name": "AC-6(9)",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": "",
      "comment": "control is reviewed",
      "state": "Reviewed",
      "updatedBy": "user1@contoso.com",
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

