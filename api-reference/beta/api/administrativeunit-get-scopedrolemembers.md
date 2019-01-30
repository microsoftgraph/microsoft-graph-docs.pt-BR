---
title: Obtenha um scopedRoleMember
description: Recupere um recurso scopedRoleMembership específico.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e961097184730922aebd4348f88b8570d5c24ca
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644095"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="bfee9-103">Obtenha um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="bfee9-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfee9-104">Recupere um recurso específico [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="bfee9-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfee9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfee9-105">Permissions</span></span>
<span data-ttu-id="bfee9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfee9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bfee9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfee9-108">Permission type</span></span>      | <span data-ttu-id="bfee9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfee9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfee9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfee9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfee9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bfee9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bfee9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfee9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfee9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfee9-113">Not supported.</span></span>    |
|<span data-ttu-id="bfee9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfee9-114">Application</span></span> | <span data-ttu-id="bfee9-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfee9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfee9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfee9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfee9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bfee9-117">Optional query parameters</span></span>
<span data-ttu-id="bfee9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bfee9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfee9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfee9-119">Request headers</span></span>
| <span data-ttu-id="bfee9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bfee9-120">Name</span></span>      |<span data-ttu-id="bfee9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfee9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfee9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfee9-122">Authorization</span></span>  | <span data-ttu-id="bfee9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfee9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfee9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfee9-125">Request body</span></span>
<span data-ttu-id="bfee9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bfee9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfee9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfee9-127">Response</span></span>

<span data-ttu-id="bfee9-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto solicitada [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfee9-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfee9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfee9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfee9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfee9-130">Request</span></span>
<span data-ttu-id="bfee9-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfee9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="bfee9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfee9-132">Response</span></span>
<span data-ttu-id="bfee9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfee9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
