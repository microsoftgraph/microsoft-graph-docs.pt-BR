---
title: Obter taskDefinition
description: Obter detalhes sobre uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8105fa16971ed468e024291f97b529f2938df96c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091533"
---
# <a name="get-taskdefinition"></a><span data-ttu-id="fa9ca-103">Obter taskDefinition</span><span class="sxs-lookup"><span data-stu-id="fa9ca-103">Get taskDefinition</span></span>

<span data-ttu-id="fa9ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa9ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa9ca-105">Obter detalhes sobre uma definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-105">Get details about a task definition.</span></span>

<span data-ttu-id="fa9ca-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="fa9ca-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa9ca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa9ca-107">Permissions</span></span>
<span data-ttu-id="fa9ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa9ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fa9ca-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="fa9ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa9ca-111">Permission type</span></span> | <span data-ttu-id="fa9ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa9ca-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fa9ca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa9ca-113">Delegated (work or school account)</span></span>| <span data-ttu-id="fa9ca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-114">Not supported.</span></span> |
|<span data-ttu-id="fa9ca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa9ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa9ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-116">Not Supported.</span></span>|
|<span data-ttu-id="fa9ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa9ca-117">Application</span></span>| <span data-ttu-id="fa9ca-118">PrintTaskDefinition. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fa9ca-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa9ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa9ca-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa9ca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa9ca-120">Request headers</span></span>
| <span data-ttu-id="fa9ca-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fa9ca-121">Name</span></span>      |<span data-ttu-id="fa9ca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa9ca-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa9ca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa9ca-123">Authorization</span></span> | <span data-ttu-id="fa9ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa9ca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa9ca-126">Request body</span></span>
<span data-ttu-id="fa9ca-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fa9ca-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa9ca-128">Response</span></span>
<span data-ttu-id="fa9ca-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa9ca-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa9ca-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa9ca-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa9ca-131">Request</span></span>
<span data-ttu-id="fa9ca-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_taskdefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
```

---

### <a name="response"></a><span data-ttu-id="fa9ca-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa9ca-133">Response</span></span>
<span data-ttu-id="fa9ca-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-134">The following is an example of the response.</span></span>
><span data-ttu-id="fa9ca-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa9ca-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 380

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
