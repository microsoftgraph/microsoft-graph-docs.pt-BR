---
title: Listar membros
description: Use essa API para obter a lista de Membros (usuário e grupo) em uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b156079035b2f2332d81e018eba40bced41d9aee
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322790"
---
# <a name="list-members"></a><span data-ttu-id="beb35-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="beb35-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beb35-104">Use essa API para obter a lista de Membros (usuário e grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="beb35-104">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="beb35-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="beb35-105">Permissions</span></span>
<span data-ttu-id="beb35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beb35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="beb35-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="beb35-108">Permission type</span></span>      | <span data-ttu-id="beb35-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="beb35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beb35-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="beb35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="beb35-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="beb35-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="beb35-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="beb35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beb35-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="beb35-113">Not supported.</span></span>    |
|<span data-ttu-id="beb35-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb35-114">Application</span></span> | <span data-ttu-id="beb35-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb35-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="beb35-116">Observação: para listar os membros de uma associação oculta em uma unidade administrativa, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="beb35-116">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="beb35-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="beb35-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="beb35-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="beb35-118">Request headers</span></span>
| <span data-ttu-id="beb35-119">Nome</span><span class="sxs-lookup"><span data-stu-id="beb35-119">Name</span></span>      |<span data-ttu-id="beb35-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="beb35-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="beb35-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="beb35-121">Authorization</span></span>  | <span data-ttu-id="beb35-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="beb35-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="beb35-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="beb35-124">Request body</span></span>
<span data-ttu-id="beb35-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="beb35-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beb35-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="beb35-126">Response</span></span>

<span data-ttu-id="beb35-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [User](../resources/user.md) e/ou [Group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="beb35-127">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="beb35-128">Em vez disso, se `$ref` você colocar no final da solicitação, a resposta conterá uma coleção de `@odata.id` links/URLs para os membros.</span><span class="sxs-lookup"><span data-stu-id="beb35-128">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="beb35-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="beb35-129">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="beb35-130">Listar objetos member</span><span class="sxs-lookup"><span data-stu-id="beb35-130">List member objects</span></span>
<span data-ttu-id="beb35-131">A solicitação a seguir listará os membros da unidade administrativa, retornando um conjunto de usuários e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="beb35-131">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="beb35-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="beb35-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a><span data-ttu-id="beb35-135">Listar referências de membros</span><span class="sxs-lookup"><span data-stu-id="beb35-135">List member references</span></span>
<span data-ttu-id="beb35-136">A solicitação a seguir listará as referências de membro da unidade administrativa, retornando uma `@odata.id` coleção de referências para os membros.</span><span class="sxs-lookup"><span data-stu-id="beb35-136">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="beb35-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="beb35-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
