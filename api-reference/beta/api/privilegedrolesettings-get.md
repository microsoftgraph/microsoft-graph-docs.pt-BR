---
title: Get privilegedRoleSettings
description: Recupere as configurações de função para a função específica. Um objeto privilegedRoleSettings será retornado.
localization_priority: Normal
ms.openlocfilehash: bc77a131a148d039bea19668a630080e6a9f816b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593726"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="5705e-104">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5705e-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5705e-105">Recupere as configurações de função para a função específica.</span><span class="sxs-lookup"><span data-stu-id="5705e-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="5705e-106">Um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.</span><span class="sxs-lookup"><span data-stu-id="5705e-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="5705e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5705e-107">Permissions</span></span>

<span data-ttu-id="5705e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5705e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5705e-110">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="5705e-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="5705e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5705e-111">Permission type</span></span>      | <span data-ttu-id="5705e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5705e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5705e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5705e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5705e-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5705e-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5705e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5705e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5705e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5705e-116">Not supported.</span></span>    |
|<span data-ttu-id="5705e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5705e-117">Application</span></span> | <span data-ttu-id="5705e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5705e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5705e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5705e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5705e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5705e-120">Optional query parameters</span></span>
<span data-ttu-id="5705e-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5705e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5705e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5705e-122">Request headers</span></span>
| <span data-ttu-id="5705e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5705e-123">Name</span></span>      |<span data-ttu-id="5705e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5705e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5705e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5705e-125">Authorization</span></span>  | <span data-ttu-id="5705e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5705e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5705e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5705e-128">Request body</span></span>
<span data-ttu-id="5705e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5705e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5705e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5705e-130">Response</span></span>

<span data-ttu-id="5705e-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5705e-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="5705e-132">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="5705e-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5705e-133">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="5705e-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="5705e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5705e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5705e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5705e-135">Request</span></span>
<span data-ttu-id="5705e-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5705e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="5705e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5705e-137">Response</span></span>
<span data-ttu-id="5705e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5705e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 228

{
  "minElevationDuration": "2016-10-19T10:37:00Z",
  "maxElavationDuration": "2016-10-19T10:37:00Z",
  "elevationDuration": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5705e-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5705e-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5705e-142">Basic</span><span class="sxs-lookup"><span data-stu-id="5705e-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedrolesettings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5705e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5705e-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedrolesettings-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrolesettings-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
