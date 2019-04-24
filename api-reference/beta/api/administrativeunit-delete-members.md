---
title: Remover um membro
description: Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 29ea8aa11850909c9e7122c55dc6c686ae9135a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459497"
---
# <a name="remove-a-member"></a><span data-ttu-id="94944-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="94944-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94944-104">Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="94944-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="94944-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="94944-105">Permissions</span></span>
<span data-ttu-id="94944-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="94944-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94944-108">Permission type</span></span>      | <span data-ttu-id="94944-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94944-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94944-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94944-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94944-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94944-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94944-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94944-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94944-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94944-113">Not supported.</span></span>    |
|<span data-ttu-id="94944-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94944-114">Application</span></span> | <span data-ttu-id="94944-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94944-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94944-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94944-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="94944-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94944-117">Request headers</span></span>
| <span data-ttu-id="94944-118">Nome</span><span class="sxs-lookup"><span data-stu-id="94944-118">Name</span></span>      |<span data-ttu-id="94944-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="94944-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94944-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="94944-120">Authorization</span></span>  | <span data-ttu-id="94944-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94944-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94944-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94944-123">Request body</span></span>
<span data-ttu-id="94944-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94944-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94944-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="94944-125">Response</span></span>

<span data-ttu-id="94944-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94944-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94944-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94944-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94944-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94944-129">Request</span></span>
<span data-ttu-id="94944-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94944-130">Here is an example of the request.</span></span> <span data-ttu-id="94944-131">No exemplo abaixo, ID1 representa o identificador para a unidade administrativa de destino e ID2 representa o identificador exclusivo para o usuário ou grupo membro a ser removido da unidade administrativa do direcionada.</span><span class="sxs-lookup"><span data-stu-id="94944-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="94944-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="94944-132">Response</span></span>
<span data-ttu-id="94944-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94944-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
