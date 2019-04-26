---
title: 'alerta: updateAlerts'
description: Atualize vários alertas em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: ad43cf3488ff0661a4b22130ae8728a00c3ea17d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322688"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="d0282-103">alerta: updateAlerts</span><span class="sxs-lookup"><span data-stu-id="d0282-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0282-104">Atualize vários alertas em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="d0282-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0282-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0282-105">Permissions</span></span>

<span data-ttu-id="d0282-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0282-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0282-108">Permission type</span></span>                        | <span data-ttu-id="d0282-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0282-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="d0282-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0282-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="d0282-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0282-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="d0282-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0282-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d0282-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0282-113">Not supported.</span></span>  |
|<span data-ttu-id="d0282-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0282-114">Application</span></span> | <span data-ttu-id="d0282-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0282-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0282-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0282-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="d0282-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0282-117">Request headers</span></span>

| <span data-ttu-id="d0282-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d0282-118">Name</span></span>          | <span data-ttu-id="d0282-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0282-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d0282-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0282-120">Authorization</span></span> | <span data-ttu-id="d0282-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d0282-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0282-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0282-122">Request body</span></span>

<span data-ttu-id="d0282-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0282-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="d0282-124">Cada entidade deve ter propriedades **ID** e **vendorInformation** .</span><span class="sxs-lookup"><span data-stu-id="d0282-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="d0282-125">Para obter detalhes sobre as propriedades que podem ser atualizadas, consulte [Update Alert](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="d0282-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="d0282-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d0282-126">Parameter</span></span>    | <span data-ttu-id="d0282-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0282-127">Type</span></span>        | <span data-ttu-id="d0282-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0282-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0282-129">valor</span><span class="sxs-lookup"><span data-stu-id="d0282-129">value</span></span>|<span data-ttu-id="d0282-130">conjunto [alerta](../resources/alert.md) </span><span class="sxs-lookup"><span data-stu-id="d0282-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="d0282-131">Conjunto de alertas a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="d0282-131">Collection of alerts to update.</span></span> <span data-ttu-id="d0282-132">Cada entidade deve ter **ID**, **vendorInformation**e outras propriedades editáveis a serem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="d0282-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="d0282-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0282-133">Response</span></span>

<span data-ttu-id="d0282-134">Se bem-sucedido, este método retorna `200, OK` o código de resposta e o objeto da coleção [Alert](../resources/alert.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0282-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0282-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0282-135">Examples</span></span>

<span data-ttu-id="d0282-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d0282-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d0282-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0282-137">Request</span></span>

<span data-ttu-id="d0282-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0282-138">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0282-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0282-139">Response</span></span>

<span data-ttu-id="d0282-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0282-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d0282-141">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d0282-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0282-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0282-142">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
