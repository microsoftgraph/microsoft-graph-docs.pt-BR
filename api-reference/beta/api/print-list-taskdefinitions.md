---
title: Listar taskDefinitions
description: Recupere uma lista de definições de tarefas que o aplicativo solicitante definido no locatário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 91d00b7773b56d4c5f522981c7a59dde3744a710
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091555"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="29f29-103">Listar taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="29f29-103">List taskDefinitions</span></span>

<span data-ttu-id="29f29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29f29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f29-105">Recupere uma lista de [definições de tarefas](../resources/printtaskdefinition.md) que o aplicativo solicitante definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="29f29-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="29f29-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="29f29-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="29f29-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="29f29-107">Permissions</span></span>
<span data-ttu-id="29f29-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="29f29-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="29f29-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29f29-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="29f29-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="29f29-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="29f29-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29f29-111">Permission type</span></span> | <span data-ttu-id="29f29-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29f29-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="29f29-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29f29-113">Delegated (work or school account)</span></span>| <span data-ttu-id="29f29-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29f29-114">Not supported.</span></span> |
|<span data-ttu-id="29f29-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29f29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29f29-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29f29-116">Not Supported.</span></span>|
|<span data-ttu-id="29f29-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29f29-117">Application</span></span>| <span data-ttu-id="29f29-118">PrintTaskDefinition. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="29f29-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29f29-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29f29-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29f29-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="29f29-120">Optional query parameters</span></span>
<span data-ttu-id="29f29-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="29f29-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="29f29-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="29f29-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="29f29-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="29f29-123">Exceptions</span></span>
<span data-ttu-id="29f29-124">Não há suporte para alguns operadores: `$count` ,,,, `$format` `$search` `$select` `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="29f29-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29f29-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29f29-125">Request headers</span></span>
| <span data-ttu-id="29f29-126">Nome</span><span class="sxs-lookup"><span data-stu-id="29f29-126">Name</span></span>      |<span data-ttu-id="29f29-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="29f29-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="29f29-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="29f29-128">Authorization</span></span> | <span data-ttu-id="29f29-129">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="29f29-129">Bearer {token}.</span></span> <span data-ttu-id="29f29-130">Required.</span><span class="sxs-lookup"><span data-stu-id="29f29-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29f29-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29f29-131">Request body</span></span>
<span data-ttu-id="29f29-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29f29-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="29f29-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="29f29-133">Response</span></span>
<span data-ttu-id="29f29-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29f29-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29f29-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29f29-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="29f29-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29f29-136">Request</span></span>
<span data-ttu-id="29f29-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29f29-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```

---

### <a name="response"></a><span data-ttu-id="29f29-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="29f29-138">Response</span></span>
<span data-ttu-id="29f29-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29f29-139">The following is an example of the response.</span></span>
><span data-ttu-id="29f29-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="29f29-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="29f29-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="29f29-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions",
  "value": [
    {
      "id": "fab143fd-ee61-4358-8558-2c7dee953982",
      "displayName": "Test TaskDefinitionName",
      "createdBy": {
        "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
        "displayName": "Requesting App Display Name"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
