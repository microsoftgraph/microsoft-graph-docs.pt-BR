---
title: Excluir connectorGroup
description: Exclua um connectorGroup.
localization_priority: Normal
ms.openlocfilehash: a0fd138281b8337df49388f4a10dc34cc02da18d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516025"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="37ad5-103">Excluir connectorGroup</span><span class="sxs-lookup"><span data-stu-id="37ad5-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37ad5-104">Exclua um connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="37ad5-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="37ad5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="37ad5-105">Permissions</span></span>
<span data-ttu-id="37ad5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37ad5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37ad5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37ad5-108">Permission type</span></span>      | <span data-ttu-id="37ad5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37ad5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37ad5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37ad5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="37ad5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37ad5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37ad5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37ad5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37ad5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37ad5-113">Not supported.</span></span>    |
|<span data-ttu-id="37ad5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37ad5-114">Application</span></span> | <span data-ttu-id="37ad5-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37ad5-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="37ad5-116">**Observação:** O grupo de conector não deve ter todos os conectores associados a ele.</span><span class="sxs-lookup"><span data-stu-id="37ad5-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="37ad5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37ad5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="37ad5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37ad5-118">Request headers</span></span>
| <span data-ttu-id="37ad5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37ad5-119">Name</span></span>       | <span data-ttu-id="37ad5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37ad5-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="37ad5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37ad5-121">Authorization</span></span>  | <span data-ttu-id="37ad5-122"> de portador</span><span class="sxs-lookup"><span data-stu-id="37ad5-122">Bearer.</span></span> <span data-ttu-id="37ad5-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="37ad5-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="37ad5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37ad5-124">Request body</span></span>
<span data-ttu-id="37ad5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37ad5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37ad5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="37ad5-126">Response</span></span>

<span data-ttu-id="37ad5-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37ad5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37ad5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37ad5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37ad5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37ad5-130">Request</span></span>
<span data-ttu-id="37ad5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37ad5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="37ad5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="37ad5-132">Response</span></span>
<span data-ttu-id="37ad5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37ad5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
