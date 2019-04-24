---
title: Adicionar um membro
description: Use esta API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1cc9ce7e091ac96ca2484c74404c3a4b04b19ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459227"
---
# <a name="add-a-member"></a><span data-ttu-id="28783-103">Adicionar um membro</span><span class="sxs-lookup"><span data-stu-id="28783-103">Add a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28783-104">Use esta API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="28783-104">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="28783-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="28783-105">Permissions</span></span>
<span data-ttu-id="28783-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="28783-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28783-108">Permission type</span></span>      | <span data-ttu-id="28783-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28783-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28783-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28783-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28783-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28783-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28783-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28783-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28783-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28783-113">Not supported.</span></span>    |
|<span data-ttu-id="28783-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28783-114">Application</span></span> | <span data-ttu-id="28783-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28783-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28783-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28783-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="28783-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28783-117">Request headers</span></span>
| <span data-ttu-id="28783-118">Nome</span><span class="sxs-lookup"><span data-stu-id="28783-118">Name</span></span>      |<span data-ttu-id="28783-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="28783-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28783-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="28783-120">Authorization</span></span>  | <span data-ttu-id="28783-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28783-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28783-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28783-123">Request body</span></span>
<span data-ttu-id="28783-124">No corpo da solicitação, forneça uma representação JSON de um [usuário](../resources/user.md), [grupo](../resources/group.md) ou [directoryobject](../resources/directoryobject.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="28783-124">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="28783-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="28783-125">Response</span></span>

<span data-ttu-id="28783-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28783-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28783-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28783-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28783-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28783-129">Request</span></span>
<span data-ttu-id="28783-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28783-130">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="28783-131">No corpo da solicitação, forneça uma representação JSON do `id` objeto [User](../resources/user.md) ou [Group](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="28783-131">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="28783-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="28783-132">Response</span></span>
<span data-ttu-id="28783-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28783-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
