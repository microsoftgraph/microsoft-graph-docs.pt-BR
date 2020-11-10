---
title: Obter informações
description: Recuperar propriedades do objeto itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8eb90b2ce1a89faf7666a0885dcbc50ca62ed4c2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969943"
---
# <a name="get-iteminsightssettings"></a><span data-ttu-id="f28b7-103">Obter itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="f28b7-103">Get itemInsightsSettings</span></span>

<span data-ttu-id="f28b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f28b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f28b7-105">Obtenha as propriedades do objeto [itemInsightsSettings](../resources/iteminsightssettings.md) .</span><span class="sxs-lookup"><span data-stu-id="f28b7-105">Get the properties of [itemInsightsSettings](../resources/iteminsightssettings.md) object.</span></span>

<span data-ttu-id="f28b7-106">Para saber como personalizar a privacidade do item insights para sua organização, confira [Personalizar a privacidade do insights](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f28b7-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="f28b7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f28b7-107">Permissions</span></span>

<span data-ttu-id="f28b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f28b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f28b7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f28b7-110">Permission type</span></span>      | <span data-ttu-id="f28b7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f28b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f28b7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f28b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f28b7-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f28b7-113">User.Read, User.ReadWrite</span></span> |
|<span data-ttu-id="f28b7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f28b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f28b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f28b7-115">Not supported.</span></span>    |
|<span data-ttu-id="f28b7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f28b7-116">Application</span></span> | <span data-ttu-id="f28b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f28b7-117">Not supported.</span></span> |

><span data-ttu-id="f28b7-118">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="f28b7-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="f28b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f28b7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="f28b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f28b7-120">Request headers</span></span>

| <span data-ttu-id="f28b7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f28b7-121">Name</span></span>       | <span data-ttu-id="f28b7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f28b7-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="f28b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f28b7-123">Authorization</span></span>  | <span data-ttu-id="f28b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f28b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f28b7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f28b7-126">Request body</span></span>

<span data-ttu-id="f28b7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f28b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f28b7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f28b7-128">Response</span></span>

<span data-ttu-id="f28b7-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [itemInsightsSettings](../resources/iteminsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f28b7-129">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="f28b7-130">**Observação:** Essa operação verifica a validade dos valores de Propriedade do recurso **itemInsightsSettings** especificado.</span><span class="sxs-lookup"><span data-stu-id="f28b7-130">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="f28b7-131">Se a propriedade **disabledForGroup** estiver definida, essa operação não verifica a existência do grupo do Azure ad correspondente.</span><span class="sxs-lookup"><span data-stu-id="f28b7-131">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="f28b7-132">Isso significa que, se você definir **disabledForGroup** como um grupo do Azure AD que não existe ou foi excluído posteriormente, essa operação não será capaz de identificar qualquer associação de grupo e desabilitar insights de item para qualquer usuário específico.</span><span class="sxs-lookup"><span data-stu-id="f28b7-132">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="f28b7-133">Se **isEnabledInOrganization** estiver definido como `true` , a operação habilitará o insights para todos os usuários da organização.</span><span class="sxs-lookup"><span data-stu-id="f28b7-133">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="f28b7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f28b7-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f28b7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f28b7-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f28b7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f28b7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="f28b7-137">C#</span><span class="sxs-lookup"><span data-stu-id="f28b7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f28b7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f28b7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f28b7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f28b7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f28b7-140">Java</span><span class="sxs-lookup"><span data-stu-id="f28b7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f28b7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f28b7-141">Response</span></span>

<span data-ttu-id="f28b7-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f28b7-142">Here is an example of the response.</span></span> 
> <span data-ttu-id="f28b7-143">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f28b7-143">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f28b7-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f28b7-144">All of the properties will be returned from an actual call.</span></span>

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


