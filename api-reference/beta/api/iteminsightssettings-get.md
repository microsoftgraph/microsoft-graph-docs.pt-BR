---
title: Obter itemInsights
description: Recuperar propriedades do objeto itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 3e8af098035d89dbcea3436c0a17721c4d9dfc48
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443836"
---
# <a name="get-iteminsightssettings"></a><span data-ttu-id="9f653-103">Obter itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="9f653-103">Get itemInsightsSettings</span></span>

<span data-ttu-id="9f653-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f653-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f653-105">Obter as propriedades do [objeto itemInsightsSettings.](../resources/iteminsightssettings.md)</span><span class="sxs-lookup"><span data-stu-id="9f653-105">Get the properties of [itemInsightsSettings](../resources/iteminsightssettings.md) object.</span></span>

<span data-ttu-id="9f653-106">Para saber como personalizar a privacidade de insights de item para sua organização, consulte [personalizar a privacidade de insights.](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="9f653-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="9f653-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f653-107">Permissions</span></span>

<span data-ttu-id="9f653-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f653-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f653-110">Permission type</span></span>      | <span data-ttu-id="9f653-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f653-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f653-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f653-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f653-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f653-113">User.Read.All, User.ReadWrite.All</span></span> |
|<span data-ttu-id="9f653-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f653-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f653-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f653-115">Not supported.</span></span>    |
|<span data-ttu-id="9f653-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f653-116">Application</span></span> | <span data-ttu-id="9f653-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f653-117">Not supported.</span></span> |

><span data-ttu-id="9f653-118">**Observação:** O uso de permissões delegadas para essa operação exige que o usuário inscreveu tenha uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="9f653-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f653-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f653-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="9f653-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f653-120">Request headers</span></span>

| <span data-ttu-id="9f653-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9f653-121">Name</span></span>       | <span data-ttu-id="9f653-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f653-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="9f653-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f653-123">Authorization</span></span>  | <span data-ttu-id="9f653-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f653-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f653-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f653-126">Request body</span></span>

<span data-ttu-id="9f653-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f653-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f653-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f653-128">Response</span></span>

<span data-ttu-id="9f653-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [itemInsightsSettings](../resources/iteminsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f653-129">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="9f653-130">**Observação:** Esta operação verifica a validade dos valores de propriedade do **recurso itemInsightsSettings** especificado.</span><span class="sxs-lookup"><span data-stu-id="9f653-130">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="9f653-131">Se a **propriedade disabledForGroup** estiver definida, essa operação não verificará a existência do Grupo do Azure AD correspondente.</span><span class="sxs-lookup"><span data-stu-id="9f653-131">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="9f653-132">Isso significa que, se você definir **disabledForGroup** para um grupo do Azure AD que não existia ou foi excluído posteriormente, essa operação não poderá identificar nenhuma associação de grupo e desabilitar informações de item para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="9f653-132">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="9f653-133">Se **isEnabledInOrganization** estiver definido como , a operação permitirá insights `true` para todos os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="9f653-133">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="9f653-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f653-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9f653-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f653-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9f653-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f653-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="9f653-137">C#</span><span class="sxs-lookup"><span data-stu-id="9f653-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f653-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f653-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f653-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f653-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f653-140">Java</span><span class="sxs-lookup"><span data-stu-id="9f653-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9f653-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f653-141">Response</span></span>

<span data-ttu-id="9f653-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f653-142">Here is an example of the response.</span></span> 
> <span data-ttu-id="9f653-143">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9f653-143">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9f653-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f653-144">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "get_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


