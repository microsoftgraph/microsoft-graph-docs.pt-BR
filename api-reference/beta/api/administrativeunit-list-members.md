---
title: Listar membros
description: Use essa API para obter a lista de membros (usuário e grupo) em uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 294cbdb96f44de5028e2f41fdb9c2c7caf9d186b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048257"
---
# <a name="list-members"></a><span data-ttu-id="99206-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="99206-103">List members</span></span>

<span data-ttu-id="99206-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99206-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99206-105">Use essa API para obter a lista de membros (usuário e grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="99206-105">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="99206-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="99206-106">Permissions</span></span>
<span data-ttu-id="99206-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99206-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99206-109">Permission type</span></span>      | <span data-ttu-id="99206-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99206-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99206-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99206-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99206-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="99206-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="99206-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99206-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99206-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99206-114">Not supported.</span></span>    |
|<span data-ttu-id="99206-115">Application</span><span class="sxs-lookup"><span data-stu-id="99206-115">Application</span></span> | <span data-ttu-id="99206-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99206-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="99206-117">Observação: para listar os membros de uma associação oculta em uma unidade administrativa, a permissão Member.Read.Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="99206-117">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="99206-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99206-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="99206-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99206-119">Request headers</span></span>
| <span data-ttu-id="99206-120">Nome</span><span class="sxs-lookup"><span data-stu-id="99206-120">Name</span></span>      |<span data-ttu-id="99206-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="99206-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99206-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="99206-122">Authorization</span></span>  | <span data-ttu-id="99206-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99206-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99206-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99206-125">Request body</span></span>
<span data-ttu-id="99206-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99206-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99206-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="99206-127">Response</span></span>

<span data-ttu-id="99206-128">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` de usuário [](../resources/user.md) e/ou grupo no corpo da resposta. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="99206-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="99206-129">Em vez disso, se você colocar no final da solicitação, a resposta conterá uma coleção de `$ref` `@odata.id` links/URLs para os membros.</span><span class="sxs-lookup"><span data-stu-id="99206-129">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="99206-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="99206-130">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="99206-131">Listar objetos membros</span><span class="sxs-lookup"><span data-stu-id="99206-131">List member objects</span></span>
<span data-ttu-id="99206-132">A solicitação a seguir lista os membros da unidade administrativa, retornando uma coleção de usuários e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="99206-132">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="99206-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99206-133">Here is an example of the response.</span></span> <span data-ttu-id="99206-134">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="99206-134">Note: The response object shown here might be shortened for readability.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="99206-135">Listar referências de membro</span><span class="sxs-lookup"><span data-stu-id="99206-135">List member references</span></span>
<span data-ttu-id="99206-136">A solicitação a seguir lista as referências de membro da unidade administrativa, retornando uma coleção de `@odata.id` referências aos membros.</span><span class="sxs-lookup"><span data-stu-id="99206-136">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="99206-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99206-137">Here is an example of the response.</span></span> <span data-ttu-id="99206-138">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="99206-138">Note: The response object shown here might be shortened for readability.</span></span>
 
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


