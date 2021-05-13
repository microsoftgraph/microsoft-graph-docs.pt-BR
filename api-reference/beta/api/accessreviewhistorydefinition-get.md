---
title: Obter accessReviewHistoryDefinition
description: Recupere um objeto accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 59a59aea65cdb26f1880c0b9876bfcdf54f30190
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474181"
---
# <a name="get-accessreviewhistorydefinition"></a><span data-ttu-id="c0de2-103">Obter accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="c0de2-103">Get accessReviewHistoryDefinition</span></span>

<span data-ttu-id="c0de2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0de2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0de2-105">Recupere um [objeto accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) pelo identificador.</span><span class="sxs-lookup"><span data-stu-id="c0de2-105">Retrieve an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object by its identifier.</span></span> <span data-ttu-id="c0de2-106">Todas as propriedades do objeto de definição de histórico de revisão de acesso são retornadas.</span><span class="sxs-lookup"><span data-stu-id="c0de2-106">All of the properties of the access review history definition object are returned.</span></span> <span data-ttu-id="c0de2-107">Se o link de download ainda for válido, ele será retornado junto com a definição.</span><span class="sxs-lookup"><span data-stu-id="c0de2-107">If the download link is still valid, it is returned along with the definition.</span></span> <span data-ttu-id="c0de2-108">Se a definição for 30 dias ou mais antiga, um erro 404 será retornado.</span><span class="sxs-lookup"><span data-stu-id="c0de2-108">If the definition is 30 days or older, a 404 error is returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0de2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0de2-109">Permissions</span></span>

<span data-ttu-id="c0de2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0de2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0de2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0de2-112">Permission type</span></span>|<span data-ttu-id="c0de2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0de2-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0de2-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0de2-114">Delegated (work or school account)</span></span>|<span data-ttu-id="c0de2-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0de2-115">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="c0de2-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0de2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0de2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0de2-117">Not supported.</span></span>|
|<span data-ttu-id="c0de2-118">Application</span><span class="sxs-lookup"><span data-stu-id="c0de2-118">Application</span></span>|<span data-ttu-id="c0de2-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0de2-119">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="c0de2-120">O usuário integrado também deve ser o criador da definição de histórico de revisão associada, um membro da função de diretório administrador global ou um membro da função de diretório Leitor Global para recuperar a definição.</span><span class="sxs-lookup"><span data-stu-id="c0de2-120">The signed-in user must also be the creator of the associated review history definition, a Global Admin directory role member, or a Global Reader directory role member to retrieve the definition.</span></span>

## <a name="http-request"></a><span data-ttu-id="c0de2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0de2-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/historyDefinitions/{definition-id}
```

## <a name="request-headers"></a><span data-ttu-id="c0de2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0de2-122">Request headers</span></span>
|<span data-ttu-id="c0de2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c0de2-123">Name</span></span>|<span data-ttu-id="c0de2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0de2-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c0de2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0de2-125">Authorization</span></span>|<span data-ttu-id="c0de2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0de2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0de2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0de2-128">Request body</span></span>
<span data-ttu-id="c0de2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0de2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0de2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0de2-130">Response</span></span>

<span data-ttu-id="c0de2-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0de2-131">If successful, this method returns a `200 OK` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0de2-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c0de2-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0de2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0de2-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c0de2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0de2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewhistorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38
```
# <a name="c"></a>[<span data-ttu-id="c0de2-135">C#</span><span class="sxs-lookup"><span data-stu-id="c0de2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewhistorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0de2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0de2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewhistorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0de2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0de2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewhistorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0de2-138">Java</span><span class="sxs-lookup"><span data-stu-id="c0de2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewhistorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c0de2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0de2-139">Response</span></span>
><span data-ttu-id="c0de2-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c0de2-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
