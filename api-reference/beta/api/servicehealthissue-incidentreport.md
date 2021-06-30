---
title: 'serviceHealthIssue: incidentReport'
description: Forneça o documento PIR (Revisão pós-incidente) de um problema de serviço especificado para locatário.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 1cf516a081108ba6588a93210e7d6c60967d8380
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209223"
---
# <a name="servicehealthissue-incidentreport"></a><span data-ttu-id="3cfff-103">serviceHealthIssue: incidentReport</span><span class="sxs-lookup"><span data-stu-id="3cfff-103">serviceHealthIssue: incidentReport</span></span>
<span data-ttu-id="3cfff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cfff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cfff-105">Forneça o documento PIR (Revisão pós-incidente) de um problema de serviço especificado para locatário.</span><span class="sxs-lookup"><span data-stu-id="3cfff-105">Provide the Post-Incident Review (PIR) document of a specified service issue for tenant.</span></span>

<span data-ttu-id="3cfff-106">A operação retornará um erro se o problema especificado não existir para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cfff-106">The operation returns an error if the specified issue doesn't exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cfff-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cfff-107">Permissions</span></span>
<span data-ttu-id="3cfff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cfff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cfff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cfff-110">Permission type</span></span>|<span data-ttu-id="3cfff-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cfff-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cfff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cfff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3cfff-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cfff-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="3cfff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cfff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cfff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cfff-115">Not supported.</span></span>|
|<span data-ttu-id="3cfff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cfff-116">Application</span></span>|<span data-ttu-id="3cfff-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cfff-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cfff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfff-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}/incidentReport
```

## <a name="request-headers"></a><span data-ttu-id="3cfff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfff-119">Request headers</span></span>
|<span data-ttu-id="3cfff-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3cfff-120">Name</span></span>|<span data-ttu-id="3cfff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cfff-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3cfff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cfff-122">Authorization</span></span>|<span data-ttu-id="3cfff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cfff-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cfff-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfff-125">Request body</span></span>
<span data-ttu-id="3cfff-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cfff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cfff-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cfff-127">Response</span></span>

<span data-ttu-id="3cfff-128">Se tiver êxito, essa função retornará um código de resposta e um `200 OK` fluxo de arquivos no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cfff-128">If successful, this function returns a `200 OK` response code and a file stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cfff-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cfff-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cfff-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfff-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3cfff-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfff-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO248163"],
  "name": "servicehealthissue_incidentreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO248163/incidentReport
```
# <a name="c"></a>[<span data-ttu-id="3cfff-132">C#</span><span class="sxs-lookup"><span data-stu-id="3cfff-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/servicehealthissue-incidentreport-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfff-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfff-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/servicehealthissue-incidentreport-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfff-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfff-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/servicehealthissue-incidentreport-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfff-135">Java</span><span class="sxs-lookup"><span data-stu-id="3cfff-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/servicehealthissue-incidentreport-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3cfff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cfff-136">Response</span></span>
><span data-ttu-id="3cfff-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3cfff-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": "Stream"
}
```

