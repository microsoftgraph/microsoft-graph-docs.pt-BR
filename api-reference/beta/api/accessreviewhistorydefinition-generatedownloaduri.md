---
title: 'accessReviewHistoryDefinition: generateDownloadUri'
description: Gere um URI que pode ser usado para recuperar dados de histórico de revisão.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2a8d8b2023b322bc67b9ef37f6e868104ef1037a
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474208"
---
# <a name="accessreviewhistorydefinition-generatedownloaduri"></a><span data-ttu-id="3b354-103">accessReviewHistoryDefinition: generateDownloadUri</span><span class="sxs-lookup"><span data-stu-id="3b354-103">accessReviewHistoryDefinition: generateDownloadUri</span></span>

<span data-ttu-id="3b354-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b354-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b354-105">Gere um URI que pode ser usado para recuperar dados de histórico de revisão para o [accessReviewHistoryDefinition](../resources/accessReviewHistoryDefinition.md)associado.</span><span class="sxs-lookup"><span data-stu-id="3b354-105">Generate a URI that can be used to retrieve review history data for the associated [accessReviewHistoryDefinition](../resources/accessReviewHistoryDefinition.md).</span></span> <span data-ttu-id="3b354-106">Esse URI é válido por um dia e pode ser recuperado buscando a propriedade **downloadUri** do objeto [accessReviewHistoryDefinition](../resources/accessReviewHistoryDefinition.md) associado.</span><span class="sxs-lookup"><span data-stu-id="3b354-106">This URI is valid for one day and can be retrieved by fetching the **downloadUri** property from the associated [accessReviewHistoryDefinition](../resources/accessReviewHistoryDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b354-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b354-107">Permissions</span></span>

<span data-ttu-id="3b354-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b354-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b354-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b354-110">Permission type</span></span>|<span data-ttu-id="3b354-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b354-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b354-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b354-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b354-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b354-113">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="3b354-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b354-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b354-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b354-115">Not supported.</span></span>|
|<span data-ttu-id="3b354-116">Application</span><span class="sxs-lookup"><span data-stu-id="3b354-116">Application</span></span>|<span data-ttu-id="3b354-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b354-117">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="3b354-118">O usuário associado também deve ser o criador da definição de histórico de revisão associada, um membro da função de diretório administrador global ou um membro da função de diretório Leitor Global para gerar o link.</span><span class="sxs-lookup"><span data-stu-id="3b354-118">The signed-in user must also be the creator of the associated review history definition, a Global Admin directory role member, or a Global Reader directory role member to generate the link.</span></span>

## <a name="http-request"></a><span data-ttu-id="3b354-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b354-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions/{definition-id}/generateDownloadUri()
```

## <a name="request-headers"></a><span data-ttu-id="3b354-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b354-120">Request headers</span></span>
|<span data-ttu-id="3b354-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3b354-121">Name</span></span>|<span data-ttu-id="3b354-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b354-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b354-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b354-123">Authorization</span></span>|<span data-ttu-id="3b354-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b354-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b354-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b354-126">Request body</span></span>
<span data-ttu-id="3b354-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b354-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b354-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b354-128">Response</span></span>

<span data-ttu-id="3b354-129">Se tiver êxito, essa ação retornará um código de resposta e `200 OK` um [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b354-129">If successful, this action returns a `200 OK` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b354-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3b354-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3b354-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b354-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3b354-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b354-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewhistorydefinition_generatedownloaduri"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38/generateDownloadUri
```
# <a name="c"></a>[<span data-ttu-id="3b354-133">C#</span><span class="sxs-lookup"><span data-stu-id="3b354-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewhistorydefinition-generatedownloaduri-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b354-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b354-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewhistorydefinition-generatedownloaduri-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b354-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b354-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewhistorydefinition-generatedownloaduri-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b354-136">Java</span><span class="sxs-lookup"><span data-stu-id="3b354-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewhistorydefinition-generatedownloaduri-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3b354-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b354-137">Response</span></span>
><span data-ttu-id="3b354-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3b354-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "done",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": "2021-04-14T00:22:58.5276552Z",
  "downloadUri": "https://contoso.com/df-erm-reports/Last quarter's group reviews April 2021-22be232e-a93d-42a3-8ac5-313cfd29a0eb.csv?sv=2015-04-05&ss=b&srt=o&sp=rl&st=2021-04-15T00:22:58.5276552Z&se=2021-03-23T19:41:38.0000000Z&spr=https&sig=84rlGCIgU4ToMn%2FFLncBXq95O8a8RsFlwQY1Knl%2Fo%2FI%3D",
  "createdBy": {
      "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
      "displayName": "MOD Administrator",
      "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
