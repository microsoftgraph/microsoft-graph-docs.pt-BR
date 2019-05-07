---
title: 'alerta: updateAlerts'
description: Atualize vários alertas em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b04227886085305103dd6a9ba6c243565d0e5a06
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636524"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="5e89d-103">alerta: updateAlerts</span><span class="sxs-lookup"><span data-stu-id="5e89d-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e89d-104">Atualize vários alertas em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="5e89d-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e89d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e89d-105">Permissions</span></span>

<span data-ttu-id="5e89d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e89d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e89d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e89d-108">Permission type</span></span>                        | <span data-ttu-id="5e89d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e89d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="5e89d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e89d-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="5e89d-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e89d-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="5e89d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e89d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5e89d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e89d-113">Not supported.</span></span>  |
|<span data-ttu-id="5e89d-114">Application</span><span class="sxs-lookup"><span data-stu-id="5e89d-114">Application</span></span> | <span data-ttu-id="5e89d-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e89d-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e89d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e89d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="5e89d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e89d-117">Request headers</span></span>

| <span data-ttu-id="5e89d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5e89d-118">Name</span></span>          | <span data-ttu-id="5e89d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e89d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5e89d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e89d-120">Authorization</span></span> | <span data-ttu-id="5e89d-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5e89d-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e89d-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e89d-122">Request body</span></span>

<span data-ttu-id="5e89d-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e89d-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="5e89d-124">Cada entidade deve ter propriedades **ID** e **vendorInformation** .</span><span class="sxs-lookup"><span data-stu-id="5e89d-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="5e89d-125">Para obter detalhes sobre as propriedades que podem ser atualizadas, consulte [Update Alert](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="5e89d-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="5e89d-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5e89d-126">Parameter</span></span>    | <span data-ttu-id="5e89d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e89d-127">Type</span></span>        | <span data-ttu-id="5e89d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e89d-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e89d-129">valor</span><span class="sxs-lookup"><span data-stu-id="5e89d-129">value</span></span>|<span data-ttu-id="5e89d-130">conjunto [alerta](../resources/alert.md) </span><span class="sxs-lookup"><span data-stu-id="5e89d-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="5e89d-131">Conjunto de alertas a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="5e89d-131">Collection of alerts to update.</span></span> <span data-ttu-id="5e89d-132">Cada entidade deve ter **ID**, **vendorInformation**e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="5e89d-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="5e89d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e89d-133">Response</span></span>

<span data-ttu-id="5e89d-134">Se bem-sucedido, este método retorna `200, OK` o código de resposta e o objeto da coleção [Alert](../resources/alert.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e89d-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e89d-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5e89d-135">Examples</span></span>

<span data-ttu-id="5e89d-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5e89d-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5e89d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e89d-137">Request</span></span>

<span data-ttu-id="5e89d-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e89d-138">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e89d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e89d-139">Response</span></span>

<span data-ttu-id="5e89d-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5e89d-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5e89d-141">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e89d-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5e89d-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e89d-142">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5e89d-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5e89d-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5e89d-144">Basic</span><span class="sxs-lookup"><span data-stu-id="5e89d-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/alert_updatealerts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e89d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e89d-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/alert_updatealerts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-updatealerts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-updatealerts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
