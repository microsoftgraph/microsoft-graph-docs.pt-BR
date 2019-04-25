---
title: Get privilegedRoleSettings
description: Recupere as configurações de função para a função específica. Um objeto privilegedRoleSettings será retornado.
localization_priority: Normal
ms.openlocfilehash: 7ecebad77acf2e090263878aacc29f00a9215fc7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546462"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="eb390-104">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="eb390-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb390-105">Recupere as configurações de função para a função específica.</span><span class="sxs-lookup"><span data-stu-id="eb390-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="eb390-106">Um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.</span><span class="sxs-lookup"><span data-stu-id="eb390-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb390-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb390-107">Permissions</span></span>

<span data-ttu-id="eb390-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb390-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eb390-110">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="eb390-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="eb390-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb390-111">Permission type</span></span>      | <span data-ttu-id="eb390-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb390-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb390-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb390-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eb390-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eb390-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eb390-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb390-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb390-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb390-116">Not supported.</span></span>    |
|<span data-ttu-id="eb390-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb390-117">Application</span></span> | <span data-ttu-id="eb390-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb390-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb390-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb390-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb390-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb390-120">Optional query parameters</span></span>
<span data-ttu-id="eb390-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eb390-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb390-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb390-122">Request headers</span></span>
| <span data-ttu-id="eb390-123">Nome</span><span class="sxs-lookup"><span data-stu-id="eb390-123">Name</span></span>      |<span data-ttu-id="eb390-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb390-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb390-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb390-125">Authorization</span></span>  | <span data-ttu-id="eb390-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb390-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb390-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb390-128">Request body</span></span>
<span data-ttu-id="eb390-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb390-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb390-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb390-130">Response</span></span>

<span data-ttu-id="eb390-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb390-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="eb390-132">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="eb390-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="eb390-133">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="eb390-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="eb390-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb390-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb390-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb390-135">Request</span></span>
<span data-ttu-id="eb390-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb390-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="eb390-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb390-137">Response</span></span>
<span data-ttu-id="eb390-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb390-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
