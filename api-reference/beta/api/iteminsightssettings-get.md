---
title: Obter itemInsights
description: Recuperar propriedades do objeto itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: dfec7c1ea7ed8befcf3480a2efadd6dfcfaa3451
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038478"
---
# <a name="get-iteminsightssettings"></a><span data-ttu-id="3ed65-103">Obter itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="3ed65-103">Get itemInsightsSettings</span></span>

<span data-ttu-id="3ed65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ed65-105">Obter as propriedades do [objeto itemInsightsSettings.](../resources/iteminsightssettings.md)</span><span class="sxs-lookup"><span data-stu-id="3ed65-105">Get the properties of [itemInsightsSettings](../resources/iteminsightssettings.md) object.</span></span>

<span data-ttu-id="3ed65-106">Para saber como personalizar a privacidade de insights de item para sua organização, consulte [personalizar a privacidade de insights.](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="3ed65-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="3ed65-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ed65-107">Permissions</span></span>

<span data-ttu-id="3ed65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ed65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ed65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ed65-110">Permission type</span></span>      | <span data-ttu-id="3ed65-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ed65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ed65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ed65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ed65-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ed65-113">User.Read.All, User.ReadWrite.All</span></span> |
|<span data-ttu-id="3ed65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ed65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ed65-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ed65-115">Not supported.</span></span>    |
|<span data-ttu-id="3ed65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ed65-116">Application</span></span> | <span data-ttu-id="3ed65-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ed65-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ed65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ed65-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="3ed65-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ed65-119">Request headers</span></span>

| <span data-ttu-id="3ed65-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3ed65-120">Name</span></span>       | <span data-ttu-id="3ed65-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ed65-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="3ed65-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ed65-122">Authorization</span></span>  | <span data-ttu-id="3ed65-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ed65-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ed65-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ed65-125">Request body</span></span>

<span data-ttu-id="3ed65-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ed65-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ed65-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ed65-127">Response</span></span>

<span data-ttu-id="3ed65-128">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [itemInsightsSettings](../resources/iteminsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ed65-128">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="3ed65-129">**Observação:** Esta operação verifica a validade dos valores de propriedade do **recurso itemInsightsSettings** especificado.</span><span class="sxs-lookup"><span data-stu-id="3ed65-129">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="3ed65-130">Se a **propriedade disabledForGroup** estiver definida, essa operação não verificará a existência do Grupo do Azure AD correspondente.</span><span class="sxs-lookup"><span data-stu-id="3ed65-130">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="3ed65-131">Isso significa que, se você definir **disabledForGroup** para um grupo do Azure AD que não existia ou foi excluído posteriormente, essa operação não poderá identificar nenhuma associação de grupo e desabilitar informações de item para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="3ed65-131">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="3ed65-132">Se **isEnabledInOrganization** estiver definido como , a operação permitirá insights `true` para todos os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="3ed65-132">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="3ed65-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ed65-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ed65-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ed65-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3ed65-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ed65-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="3ed65-136">C#</span><span class="sxs-lookup"><span data-stu-id="3ed65-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ed65-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ed65-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ed65-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ed65-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ed65-139">Java</span><span class="sxs-lookup"><span data-stu-id="3ed65-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3ed65-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ed65-140">Response</span></span>

<span data-ttu-id="3ed65-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ed65-141">Here is an example of the response.</span></span> 
> <span data-ttu-id="3ed65-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3ed65-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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


