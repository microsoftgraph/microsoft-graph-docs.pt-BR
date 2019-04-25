---
title: Atualizar oAuth2PermissionGrant
description: Atualize as propriedades do objeto oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: fb990c56b4d7ae62ac35935a91d69688b96bff28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540202"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="f62c6-103">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f62c6-103">Update oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f62c6-104">Atualize as propriedades do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="f62c6-104">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f62c6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f62c6-105">Permissions</span></span>

<span data-ttu-id="f62c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f62c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f62c6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f62c6-108">Permission type</span></span>      | <span data-ttu-id="f62c6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f62c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f62c6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f62c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f62c6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f62c6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f62c6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f62c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f62c6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f62c6-113">Not supported.</span></span>    |
|<span data-ttu-id="f62c6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f62c6-114">Application</span></span> | <span data-ttu-id="f62c6-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f62c6-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f62c6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f62c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f62c6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f62c6-117">Request headers</span></span>
| <span data-ttu-id="f62c6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f62c6-118">Name</span></span>       | <span data-ttu-id="f62c6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f62c6-119">Type</span></span> | <span data-ttu-id="f62c6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f62c6-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f62c6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f62c6-121">Authorization</span></span>  | <span data-ttu-id="f62c6-122">string</span><span class="sxs-lookup"><span data-stu-id="f62c6-122">string</span></span>  | <span data-ttu-id="f62c6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f62c6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f62c6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f62c6-125">Request body</span></span>
<span data-ttu-id="f62c6-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f62c6-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f62c6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f62c6-129">Property</span></span>     | <span data-ttu-id="f62c6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f62c6-130">Type</span></span>   |<span data-ttu-id="f62c6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f62c6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f62c6-132">scope</span><span class="sxs-lookup"><span data-stu-id="f62c6-132">scope</span></span>|<span data-ttu-id="f62c6-133">String</span><span class="sxs-lookup"><span data-stu-id="f62c6-133">String</span></span>| <span data-ttu-id="f62c6-134">Especifica o valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="f62c6-134">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="f62c6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f62c6-135">Response</span></span>

<span data-ttu-id="f62c6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f62c6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f62c6-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f62c6-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f62c6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f62c6-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
##### <a name="response"></a><span data-ttu-id="f62c6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f62c6-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
