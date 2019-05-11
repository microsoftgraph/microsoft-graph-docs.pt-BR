---
title: Atualizar secureScoreControlProfile
description: Atualize um objeto secureScoreControlProfile editável em qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
author: preetikr
localization_priority: Normal
ms.openlocfilehash: 79d958e3f2bd04be8dab2d8fe0bda6117f487973
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951283"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="c85ba-103">Atualizar secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="c85ba-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="c85ba-104">Atualize um objeto **secureScoreControlProfile** editável em qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="c85ba-104">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c85ba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c85ba-105">Permissions</span></span>

<span data-ttu-id="c85ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c85ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c85ba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c85ba-108">Permission type</span></span>      | <span data-ttu-id="c85ba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c85ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c85ba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c85ba-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="c85ba-111">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="c85ba-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="c85ba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c85ba-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c85ba-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c85ba-113">Not supported.</span></span>  |
|<span data-ttu-id="c85ba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c85ba-114">Application</span></span> | <span data-ttu-id="c85ba-115">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="c85ba-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c85ba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c85ba-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c85ba-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c85ba-117">Request headers</span></span>

| <span data-ttu-id="c85ba-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c85ba-118">Name</span></span>       | <span data-ttu-id="c85ba-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c85ba-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c85ba-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c85ba-120">Authorization</span></span>  | <span data-ttu-id="c85ba-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="c85ba-121">Bearer {code}.</span></span> <span data-ttu-id="c85ba-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c85ba-122">Required.</span></span>|
|<span data-ttu-id="c85ba-123">Preferir</span><span class="sxs-lookup"><span data-stu-id="c85ba-123">Prefer</span></span> | <span data-ttu-id="c85ba-124">Return = representação.</span><span class="sxs-lookup"><span data-stu-id="c85ba-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c85ba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c85ba-125">Request body</span></span>

<span data-ttu-id="c85ba-126">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c85ba-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c85ba-127">O corpo **deve** conter a `vendorInformation` Propriedade com os `provider` campos `vendor` válidos e.</span><span class="sxs-lookup"><span data-stu-id="c85ba-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="c85ba-128">A tabela a seguir lista os campos que podem ser atualizados para um **secureScoreControlProfile**.</span><span class="sxs-lookup"><span data-stu-id="c85ba-128">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="c85ba-129">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="c85ba-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="c85ba-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c85ba-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c85ba-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c85ba-131">Property</span></span>   | <span data-ttu-id="c85ba-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c85ba-132">Type</span></span> |<span data-ttu-id="c85ba-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c85ba-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c85ba-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="c85ba-134">assignedTo</span></span>|<span data-ttu-id="c85ba-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c85ba-135">String</span></span>|<span data-ttu-id="c85ba-136">Nome do analista ao qual o controle é atribuído para a triagem, implementação ou correção.</span><span class="sxs-lookup"><span data-stu-id="c85ba-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="c85ba-137">comment</span><span class="sxs-lookup"><span data-stu-id="c85ba-137">comment</span></span>|<span data-ttu-id="c85ba-138">String</span><span class="sxs-lookup"><span data-stu-id="c85ba-138">String</span></span>|<span data-ttu-id="c85ba-139">Comentários de analista sobre o controle (para o gerenciamento de controle de clientes).</span><span class="sxs-lookup"><span data-stu-id="c85ba-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="c85ba-140">state</span><span class="sxs-lookup"><span data-stu-id="c85ba-140">state</span></span>| <span data-ttu-id="c85ba-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c85ba-141">String</span></span>|<span data-ttu-id="c85ba-142">Configuração orientada pelo analista no controle.</span><span class="sxs-lookup"><span data-stu-id="c85ba-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="c85ba-143">Os valores possíveis são: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span><span class="sxs-lookup"><span data-stu-id="c85ba-143">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="c85ba-144">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="c85ba-144">vendorInformation</span></span> | [<span data-ttu-id="c85ba-145">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="c85ba-145">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="c85ba-146">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore;).</span><span class="sxs-lookup"><span data-stu-id="c85ba-146">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="c85ba-147">**Os campos Provider e Vendor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="c85ba-147">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="c85ba-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c85ba-148">Response</span></span>

<span data-ttu-id="c85ba-149">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c85ba-149">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="c85ba-150">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c85ba-150">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c85ba-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c85ba-151">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="c85ba-152">Exemplo 1: solicitação sem cabeçalho de preferência</span><span class="sxs-lookup"><span data-stu-id="c85ba-152">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="c85ba-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c85ba-153">Request</span></span>

<span data-ttu-id="c85ba-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c85ba-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
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

### <a name="response"></a><span data-ttu-id="c85ba-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="c85ba-155">Response</span></span>

<span data-ttu-id="c85ba-156">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c85ba-156">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c85ba-157">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="c85ba-157">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c85ba-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="c85ba-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_update-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="c85ba-159">Exemplo 2: solicitação com cabeçalho preferencial</span><span class="sxs-lookup"><span data-stu-id="c85ba-159">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="c85ba-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c85ba-160">Request</span></span>

<span data-ttu-id="c85ba-161">O exemplo a seguir mostra uma solicitação que inclui `Prefer` o cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c85ba-161">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
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

#### <a name="response"></a><span data-ttu-id="c85ba-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c85ba-162">Response</span></span>

<span data-ttu-id="c85ba-163">Veja a seguir um exemplo da resposta quando o cabeçalho de `Prefer: return=representation` solicitação opcional é usado.</span><span class="sxs-lookup"><span data-stu-id="c85ba-163">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="c85ba-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c85ba-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/v1.0/api/securescorecontrolprofile-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/securescorecontrolprofile-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
