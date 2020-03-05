---
title: 'alerta: updateAlerts'
description: Atualize vários alertas em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 684c96aeb0f297c783343001a1ab00bc82f9da63
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441631"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="7da2f-103">alerta: updateAlerts</span><span class="sxs-lookup"><span data-stu-id="7da2f-103">alert: updateAlerts</span></span>

<span data-ttu-id="7da2f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7da2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7da2f-105">Atualize vários alertas em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="7da2f-105">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="7da2f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7da2f-106">Permissions</span></span>

<span data-ttu-id="7da2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7da2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7da2f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7da2f-109">Permission type</span></span>                        | <span data-ttu-id="7da2f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7da2f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="7da2f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7da2f-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="7da2f-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7da2f-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="7da2f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7da2f-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7da2f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7da2f-114">Not supported.</span></span>  |
|<span data-ttu-id="7da2f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7da2f-115">Application</span></span> | <span data-ttu-id="7da2f-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7da2f-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7da2f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7da2f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="7da2f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7da2f-118">Request headers</span></span>

| <span data-ttu-id="7da2f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7da2f-119">Name</span></span>          | <span data-ttu-id="7da2f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7da2f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7da2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7da2f-121">Authorization</span></span> | <span data-ttu-id="7da2f-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7da2f-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7da2f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7da2f-123">Request body</span></span>

<span data-ttu-id="7da2f-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7da2f-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="7da2f-125">Cada entidade deve ter propriedades **ID** e **vendorInformation** .</span><span class="sxs-lookup"><span data-stu-id="7da2f-125">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="7da2f-126">Para obter detalhes sobre as propriedades que podem ser atualizadas, consulte [Update Alert](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="7da2f-126">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="7da2f-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7da2f-127">Parameter</span></span>    | <span data-ttu-id="7da2f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="7da2f-128">Type</span></span>        | <span data-ttu-id="7da2f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7da2f-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7da2f-130">valor</span><span class="sxs-lookup"><span data-stu-id="7da2f-130">value</span></span>|<span data-ttu-id="7da2f-131">conjunto [alerta](../resources/alert.md) </span><span class="sxs-lookup"><span data-stu-id="7da2f-131">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="7da2f-132">Conjunto de alertas a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="7da2f-132">Collection of alerts to update.</span></span> <span data-ttu-id="7da2f-133">Cada entidade deve ter **ID**, **vendorInformation**e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="7da2f-133">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="7da2f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7da2f-134">Response</span></span>

<span data-ttu-id="7da2f-135">Se bem-sucedido, este método retorna `200, OK` o código de resposta e o objeto da coleção [Alert](../resources/alert.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7da2f-135">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7da2f-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7da2f-136">Examples</span></span>

<span data-ttu-id="7da2f-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7da2f-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7da2f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7da2f-138">Request</span></span>

<span data-ttu-id="7da2f-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7da2f-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7da2f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="7da2f-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7da2f-141">C#</span><span class="sxs-lookup"><span data-stu-id="7da2f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7da2f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7da2f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7da2f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7da2f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7da2f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7da2f-144">Response</span></span>

<span data-ttu-id="7da2f-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7da2f-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7da2f-146">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7da2f-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7da2f-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7da2f-147">All the properties will be returned from an actual call.</span></span>

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
