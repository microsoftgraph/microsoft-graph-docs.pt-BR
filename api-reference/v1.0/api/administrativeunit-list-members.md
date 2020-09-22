---
title: Listar membros
description: Use essa API para obter a lista de Membros (usuário e grupo) em uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b1703e5c372ecd00ddbe12ecf6d33612e177698
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020199"
---
# <a name="list-members"></a><span data-ttu-id="cfb84-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="cfb84-103">List members</span></span>

<span data-ttu-id="cfb84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfb84-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfb84-105">Use essa API para obter a lista de Membros (usuário e grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="cfb84-105">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfb84-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfb84-106">Permissions</span></span>
<span data-ttu-id="cfb84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfb84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfb84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfb84-109">Permission type</span></span>      | <span data-ttu-id="cfb84-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfb84-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfb84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfb84-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cfb84-112">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="cfb84-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cfb84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfb84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfb84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfb84-114">Not supported.</span></span>    |
|<span data-ttu-id="cfb84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfb84-115">Application</span></span> | <span data-ttu-id="cfb84-116">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cfb84-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="cfb84-117">Observação: para listar os membros de uma associação oculta em uma unidade administrativa, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="cfb84-117">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="cfb84-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfb84-118">HTTP request</span></span>

```http
GET /directory/administrativeUnits/{id}/members
GET /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cfb84-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfb84-119">Request headers</span></span>
| <span data-ttu-id="cfb84-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cfb84-120">Name</span></span>      |<span data-ttu-id="cfb84-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfb84-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cfb84-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfb84-122">Authorization</span></span>  | <span data-ttu-id="cfb84-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfb84-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfb84-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfb84-125">Request body</span></span>
<span data-ttu-id="cfb84-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cfb84-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfb84-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfb84-127">Response</span></span>

<span data-ttu-id="cfb84-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [User](../resources/user.md) e/ou [Group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfb84-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="cfb84-129">Em vez disso, se você colocar `$ref` no final da solicitação, a resposta conterá uma coleção de `@odata.id` links/URLs para os membros.</span><span class="sxs-lookup"><span data-stu-id="cfb84-129">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="cfb84-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cfb84-130">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="cfb84-131">Listar objetos member</span><span class="sxs-lookup"><span data-stu-id="cfb84-131">List member objects</span></span>
<span data-ttu-id="cfb84-132">A solicitação a seguir listará os membros da unidade administrativa, retornando um conjunto de usuários e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="cfb84-132">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members
```

<span data-ttu-id="cfb84-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfb84-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="cfb84-136">Listar referências de membros</span><span class="sxs-lookup"><span data-stu-id="cfb84-136">List member references</span></span>
<span data-ttu-id="cfb84-137">A solicitação a seguir listará as referências de membro da unidade administrativa, retornando uma coleção de `@odata.id` referências para os membros.</span><span class="sxs-lookup"><span data-stu-id="cfb84-137">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="cfb84-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfb84-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
