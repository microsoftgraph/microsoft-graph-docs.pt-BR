---
title: Excluir privilegedRoleAssignment
description: Exclua privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 2b98509457d7e26b4b65d42840f04550429bcc95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526743"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="30442-103">Excluir privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="30442-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30442-104">Exclua [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="30442-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="30442-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="30442-105">Permissions</span></span>
<span data-ttu-id="30442-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="30442-108">O solicitante precisa ter a função de _Administrador com privilégios de função_ .</span><span class="sxs-lookup"><span data-stu-id="30442-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="30442-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30442-109">Permission type</span></span>      | <span data-ttu-id="30442-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30442-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30442-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30442-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30442-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="30442-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="30442-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30442-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30442-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30442-114">Not supported.</span></span>    |
|<span data-ttu-id="30442-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30442-115">Application</span></span> | <span data-ttu-id="30442-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30442-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30442-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30442-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="30442-118">Observe que ``<id>`` está no formato de 'userId_roleId', onde userId é a cadeia de caracteres do GUID para id de usuário do Windows Azure AD e roleId é a cadeia de caracteres do GUID para id de função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="30442-118">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30442-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30442-119">Request headers</span></span>
| <span data-ttu-id="30442-120">Nome</span><span class="sxs-lookup"><span data-stu-id="30442-120">Name</span></span>       | <span data-ttu-id="30442-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="30442-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="30442-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="30442-122">Authorization</span></span>  | <span data-ttu-id="30442-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30442-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30442-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30442-125">Request body</span></span>
<span data-ttu-id="30442-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30442-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30442-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="30442-127">Response</span></span>

<span data-ttu-id="30442-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30442-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="30442-130">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="30442-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="30442-131">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="30442-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="30442-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30442-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30442-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30442-133">Request</span></span>
<span data-ttu-id="30442-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30442-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="30442-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="30442-135">Response</span></span>
<span data-ttu-id="30442-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30442-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
