---
title: Obter privilegedRoleSettings
description: Recupere as configurações de função para uma determinada função. Um objeto privilegedRoleSettings será retornado.
ms.openlocfilehash: c064e2eb11a4e91247894338c43c7c6dd9f9dcc3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034427"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="c4ddc-104">Obter privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c4ddc-104">Get privilegedRoleSettings</span></span>

> <span data-ttu-id="c4ddc-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4ddc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4ddc-107">Recupere as configurações de função para uma determinada função.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-107">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="c4ddc-108">Um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4ddc-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="c4ddc-109">Permissions</span></span>

<span data-ttu-id="c4ddc-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4ddc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c4ddc-112">O solicitante precisa ter uma das seguintes funções: _Leitor de segurança_, _Administrador Global_, _Administrador de segurança_ou _Administrador com privilégios de função_.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="c4ddc-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4ddc-113">Permission type</span></span>      | <span data-ttu-id="c4ddc-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4ddc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4ddc-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4ddc-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c4ddc-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4ddc-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4ddc-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4ddc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4ddc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-118">Not supported.</span></span>    |
|<span data-ttu-id="c4ddc-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4ddc-119">Application</span></span> | <span data-ttu-id="c4ddc-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4ddc-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ddc-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4ddc-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4ddc-122">Optional query parameters</span></span>
<span data-ttu-id="c4ddc-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4ddc-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ddc-124">Request headers</span></span>
| <span data-ttu-id="c4ddc-125">Nome</span><span class="sxs-lookup"><span data-stu-id="c4ddc-125">Name</span></span>      |<span data-ttu-id="c4ddc-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4ddc-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4ddc-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4ddc-127">Authorization</span></span>  | <span data-ttu-id="c4ddc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4ddc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ddc-130">Request body</span></span>
<span data-ttu-id="c4ddc-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4ddc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ddc-132">Response</span></span>

<span data-ttu-id="c4ddc-133">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [privilegedRoleSettings](../resources/privilegedrolesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-133">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="c4ddc-134">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c4ddc-135">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c4ddc-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4ddc-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4ddc-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ddc-137">Request</span></span>
<span data-ttu-id="c4ddc-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="c4ddc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ddc-139">Response</span></span>
<span data-ttu-id="c4ddc-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4ddc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->