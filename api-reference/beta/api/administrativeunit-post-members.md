---
title: Adicionar um membro
description: Use essa API para adicionar um membro (usuário ou grupo) para uma unidade administrativa.
ms.openlocfilehash: d969be353a1ae41f0b1ba0d302b497596804e325
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034073"
---
# <a name="add-a-member"></a><span data-ttu-id="bfe76-103">Adicionar um membro</span><span class="sxs-lookup"><span data-stu-id="bfe76-103">Add a member</span></span>

> <span data-ttu-id="bfe76-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bfe76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfe76-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bfe76-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfe76-106">Use essa API para adicionar um membro (usuário ou grupo) para uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="bfe76-106">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="bfe76-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="bfe76-107">Permissions</span></span>
<span data-ttu-id="bfe76-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfe76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bfe76-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfe76-110">Permission type</span></span>      | <span data-ttu-id="bfe76-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfe76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfe76-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfe76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bfe76-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bfe76-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bfe76-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfe76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfe76-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfe76-115">Not supported.</span></span>    |
|<span data-ttu-id="bfe76-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfe76-116">Application</span></span> | <span data-ttu-id="bfe76-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfe76-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfe76-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfe76-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bfe76-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfe76-119">Request headers</span></span>
| <span data-ttu-id="bfe76-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bfe76-120">Name</span></span>      |<span data-ttu-id="bfe76-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfe76-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfe76-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfe76-122">Authorization</span></span>  | <span data-ttu-id="bfe76-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfe76-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfe76-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfe76-125">Request body</span></span>
<span data-ttu-id="bfe76-126">No corpo da solicitação, fornece uma representação JSON de um [usuário](../resources/user.md), [grupo](../resources/group.md) ou [directoryObject](../resources/directoryobject.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="bfe76-126">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="bfe76-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfe76-127">Response</span></span>

<span data-ttu-id="bfe76-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfe76-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfe76-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfe76-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfe76-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfe76-131">Request</span></span>
<span data-ttu-id="bfe76-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfe76-132">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="bfe76-133">No corpo da solicitação, fornecer uma representação JSON do `id` do objeto de [usuário](../resources/user.md) ou [grupo](../resources/group.md) que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="bfe76-133">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="bfe76-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfe76-134">Response</span></span>
<span data-ttu-id="bfe76-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfe76-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
