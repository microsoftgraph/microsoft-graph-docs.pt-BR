---
title: 'serviceHealthIssue: incidentReport'
description: Forneça o documento PIR (Revisão pós-incidente) de um problema de serviço especificado para locatário.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 155c5d83c33a5276a127d33684cd8724d65ddf79
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151619"
---
# <a name="servicehealthissue-incidentreport"></a><span data-ttu-id="f7fe1-103">serviceHealthIssue: incidentReport</span><span class="sxs-lookup"><span data-stu-id="f7fe1-103">serviceHealthIssue: incidentReport</span></span>
<span data-ttu-id="f7fe1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7fe1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7fe1-105">Forneça o documento PIR (Revisão pós-incidente) de um problema de serviço especificado para locatário.</span><span class="sxs-lookup"><span data-stu-id="f7fe1-105">Provide the Post-Incident Review (PIR) document of a specified service issue for tenant.</span></span>

<span data-ttu-id="f7fe1-106">A operação retornará um erro se o problema especificado não existir para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7fe1-106">The operation returns an error if the specified issue doesn't exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7fe1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7fe1-107">Permissions</span></span>
<span data-ttu-id="f7fe1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7fe1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7fe1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7fe1-110">Permission type</span></span>|<span data-ttu-id="f7fe1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7fe1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7fe1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7fe1-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7fe1-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="f7fe1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7fe1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7fe1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7fe1-115">Not supported.</span></span>|
|<span data-ttu-id="f7fe1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7fe1-116">Application</span></span>|<span data-ttu-id="f7fe1-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7fe1-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7fe1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7fe1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}/incidentReport
```

## <a name="request-headers"></a><span data-ttu-id="f7fe1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fe1-119">Request headers</span></span>
|<span data-ttu-id="f7fe1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f7fe1-120">Name</span></span>|<span data-ttu-id="f7fe1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7fe1-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7fe1-122">Authorization</span></span>|<span data-ttu-id="f7fe1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7fe1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fe1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fe1-125">Request body</span></span>
<span data-ttu-id="f7fe1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7fe1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7fe1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7fe1-127">Response</span></span>

<span data-ttu-id="f7fe1-128">Se tiver êxito, essa função retornará um código de resposta e um `200 OK` fluxo de arquivos no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7fe1-128">If successful, this function returns a `200 OK` response code and a file stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7fe1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7fe1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7fe1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fe1-130">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO248163"],
  "name": "servicehealthissue_incidentreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO248163/incidentReport
```


### <a name="response"></a><span data-ttu-id="f7fe1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7fe1-131">Response</span></span>
><span data-ttu-id="f7fe1-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7fe1-132">**Note:** The response object shown here might be shortened for readability.</span></span>
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

