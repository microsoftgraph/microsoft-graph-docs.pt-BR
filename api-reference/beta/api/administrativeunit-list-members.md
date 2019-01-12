---
title: Listar membros
description: Use essa API para obter os membros da lista (de usuário e de grupo) em uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7513192986e8df482209c4f8630c8dab8450e614
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917206"
---
# <a name="list-members"></a><span data-ttu-id="dba91-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="dba91-103">List members</span></span>

> <span data-ttu-id="dba91-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dba91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dba91-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dba91-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dba91-106">Use essa API para obter os membros da lista (de usuário e de grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="dba91-106">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="dba91-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dba91-107">Permissions</span></span>
<span data-ttu-id="dba91-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dba91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dba91-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dba91-110">Permission type</span></span>      | <span data-ttu-id="dba91-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dba91-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dba91-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dba91-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dba91-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dba91-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dba91-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dba91-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dba91-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dba91-115">Not supported.</span></span>    |
|<span data-ttu-id="dba91-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dba91-116">Application</span></span> | <span data-ttu-id="dba91-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba91-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="dba91-118">Observação: Para listar os membros de uma associação oculta em uma unidade administrativa, a permissão de Member.Read.Hidden é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dba91-118">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="dba91-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dba91-119">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="dba91-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dba91-120">Request headers</span></span>
| <span data-ttu-id="dba91-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dba91-121">Name</span></span>      |<span data-ttu-id="dba91-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dba91-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dba91-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dba91-123">Authorization</span></span>  | <span data-ttu-id="dba91-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dba91-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dba91-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dba91-126">Request body</span></span>
<span data-ttu-id="dba91-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dba91-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dba91-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dba91-128">Response</span></span>

<span data-ttu-id="dba91-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [usuário](../resources/user.md) e/ou [grupo](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dba91-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="dba91-130">Em vez disso, se você colocar `$ref` ao final da solicitação, a resposta conterá uma coleção de `@odata.id` links/URLs aos membros.</span><span class="sxs-lookup"><span data-stu-id="dba91-130">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="dba91-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dba91-131">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="dba91-132">Objetos de membros da lista</span><span class="sxs-lookup"><span data-stu-id="dba91-132">List member objects</span></span>
<span data-ttu-id="dba91-133">A seguinte solicitação listará os membros da unidade administrativa, retornando uma coleção de usuários e/ou em grupos.</span><span class="sxs-lookup"><span data-stu-id="dba91-133">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="dba91-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dba91-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="dba91-137">Referências de membro de lista</span><span class="sxs-lookup"><span data-stu-id="dba91-137">List member references</span></span>
<span data-ttu-id="dba91-138">A seguinte solicitação listará as referências de membro da unidade administrativa, retornando uma coleção de `@odata.id` referências aos membros.</span><span class="sxs-lookup"><span data-stu-id="dba91-138">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="dba91-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dba91-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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
