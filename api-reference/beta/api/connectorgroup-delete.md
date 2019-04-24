---
title: Excluir um ou de conector
description: Excluir um conector.
localization_priority: Normal
ms.openlocfilehash: a0fd138281b8337df49388f4a10dc34cc02da18d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455909"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="05af6-103">Excluir um ou de conector</span><span class="sxs-lookup"><span data-stu-id="05af6-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05af6-104">Excluir um conector.</span><span class="sxs-lookup"><span data-stu-id="05af6-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="05af6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="05af6-105">Permissions</span></span>
<span data-ttu-id="05af6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05af6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05af6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05af6-108">Permission type</span></span>      | <span data-ttu-id="05af6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05af6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05af6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05af6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05af6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05af6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05af6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05af6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05af6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05af6-113">Not supported.</span></span>    |
|<span data-ttu-id="05af6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05af6-114">Application</span></span> | <span data-ttu-id="05af6-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05af6-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="05af6-116">**Observação:** O grupo de conectores não deve ter conectores associados a ele.</span><span class="sxs-lookup"><span data-stu-id="05af6-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="05af6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05af6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="05af6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05af6-118">Request headers</span></span>
| <span data-ttu-id="05af6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="05af6-119">Name</span></span>       | <span data-ttu-id="05af6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="05af6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="05af6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="05af6-121">Authorization</span></span>  | <span data-ttu-id="05af6-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="05af6-122">Bearer.</span></span> <span data-ttu-id="05af6-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="05af6-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="05af6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05af6-124">Request body</span></span>
<span data-ttu-id="05af6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05af6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05af6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="05af6-126">Response</span></span>

<span data-ttu-id="05af6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05af6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05af6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05af6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05af6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05af6-130">Request</span></span>
<span data-ttu-id="05af6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05af6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="05af6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="05af6-132">Response</span></span>
<span data-ttu-id="05af6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05af6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
