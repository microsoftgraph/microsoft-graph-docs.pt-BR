---
title: 'alert: updateAlerts'
description: Atualize vários alertas em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 86c391f0684ebad30ef5abab0c3a7e8746445a32
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048180"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="985f7-103">alert: updateAlerts</span><span class="sxs-lookup"><span data-stu-id="985f7-103">alert: updateAlerts</span></span>

<span data-ttu-id="985f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="985f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="985f7-105">Atualize vários alertas em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="985f7-105">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="985f7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="985f7-106">Permissions</span></span>

<span data-ttu-id="985f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="985f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="985f7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="985f7-109">Permission type</span></span>                        | <span data-ttu-id="985f7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="985f7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="985f7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="985f7-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="985f7-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="985f7-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="985f7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="985f7-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="985f7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="985f7-114">Not supported.</span></span>  |
|<span data-ttu-id="985f7-115">Application</span><span class="sxs-lookup"><span data-stu-id="985f7-115">Application</span></span> | <span data-ttu-id="985f7-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="985f7-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="985f7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="985f7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="985f7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="985f7-118">Request headers</span></span>

| <span data-ttu-id="985f7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="985f7-119">Name</span></span>          | <span data-ttu-id="985f7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="985f7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="985f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="985f7-121">Authorization</span></span> | <span data-ttu-id="985f7-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="985f7-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="985f7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="985f7-123">Request body</span></span>

<span data-ttu-id="985f7-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="985f7-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="985f7-125">Cada entidade deve ter **propriedades id** e **vendorInformation.**</span><span class="sxs-lookup"><span data-stu-id="985f7-125">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="985f7-126">Para obter detalhes sobre as propriedades que podem ser atualizadas, consulte [update alert](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="985f7-126">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="985f7-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="985f7-127">Parameter</span></span>    | <span data-ttu-id="985f7-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="985f7-128">Type</span></span>        | <span data-ttu-id="985f7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="985f7-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="985f7-130">valor</span><span class="sxs-lookup"><span data-stu-id="985f7-130">value</span></span>|<span data-ttu-id="985f7-131">conjunto [alerta](../resources/alert.md) </span><span class="sxs-lookup"><span data-stu-id="985f7-131">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="985f7-132">Coleção de alertas a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="985f7-132">Collection of alerts to update.</span></span> <span data-ttu-id="985f7-133">Cada entidade deve ter **id,** **vendorInformation** e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="985f7-133">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="985f7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="985f7-134">Response</span></span>

<span data-ttu-id="985f7-135">Se tiver êxito, este método retornará o código de resposta e o objeto `200, OK` [da](../resources/alert.md) coleção de alertas no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="985f7-135">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="985f7-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="985f7-136">Examples</span></span>

<span data-ttu-id="985f7-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="985f7-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="985f7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="985f7-138">Request</span></span>

<span data-ttu-id="985f7-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="985f7-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="985f7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="985f7-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts",
   "isCollection": "true"
}-->

```http
POST https://graph.microsoft.com/beta/security/alerts/updateAlerts
Content-type: application/json

{
  "value": [
    {
      "assignedTo": "String",
      "closedDateTime": "String (timestamp)",
      "comments": ["String"],
      "feedback": {"@odata.type": "microsoft.graph.alertFeedback"},
      "id": "String (identifier)",
      "status": {"@odata.type": "microsoft.graph.alertStatus"},
      "tags": ["String"],
      "vendorInformation":
        {
          "provider": "String",
          "vendor": "String"
        }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="985f7-141">C#</span><span class="sxs-lookup"><span data-stu-id="985f7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="985f7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="985f7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="985f7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="985f7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="985f7-144">Java</span><span class="sxs-lookup"><span data-stu-id="985f7-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/alert-updatealerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="985f7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="985f7-145">Response</span></span>

<span data-ttu-id="985f7-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="985f7-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="985f7-147">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="985f7-147">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


