---
title: Obter um membro
description: Use essa API para obter um membro específico (usuário ou grupo) em uma unidade administrativa.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a9752d37fed21ebadbd0e05cc30831b13f30ef5
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917946"
---
# <a name="get-a-member"></a><span data-ttu-id="30710-103">Obter um membro</span><span class="sxs-lookup"><span data-stu-id="30710-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30710-104">Use essa API para obter um membro específico (usuário ou grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="30710-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="30710-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="30710-105">Permissions</span></span>
<span data-ttu-id="30710-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="30710-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30710-108">Permission type</span></span>      | <span data-ttu-id="30710-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30710-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30710-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30710-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30710-111">AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="30710-111">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="30710-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30710-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30710-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30710-113">Not supported.</span></span>    |
|<span data-ttu-id="30710-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30710-114">Application</span></span> | <span data-ttu-id="30710-115">AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="30710-115">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30710-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30710-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="30710-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30710-117">Request headers</span></span>
| <span data-ttu-id="30710-118">Nome</span><span class="sxs-lookup"><span data-stu-id="30710-118">Name</span></span>      |<span data-ttu-id="30710-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="30710-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30710-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="30710-120">Authorization</span></span>  | <span data-ttu-id="30710-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30710-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30710-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30710-123">Request body</span></span>
<span data-ttu-id="30710-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30710-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30710-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="30710-125">Response</span></span>

<span data-ttu-id="30710-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [User](../resources/user.md) ou [Group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30710-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30710-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30710-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30710-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30710-128">Request</span></span>
<span data-ttu-id="30710-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30710-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="30710-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="30710-130">Response</span></span>
<span data-ttu-id="30710-131">Veja um exemplo de Respone.</span><span class="sxs-lookup"><span data-stu-id="30710-131">Here is an example of the respone.</span></span> <span data-ttu-id="30710-132">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="30710-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="30710-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30710-133">All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```
