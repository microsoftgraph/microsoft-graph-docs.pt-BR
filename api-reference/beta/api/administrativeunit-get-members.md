---
title: Obter um membro
description: Use essa API para obter um membro específico (usuário ou grupo) em uma unidade administrativa.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7db3137c8e1862d0b5c8ebf42c8e8a0efac65f27
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991985"
---
# <a name="get-a-member"></a><span data-ttu-id="6971a-103">Obter um membro</span><span class="sxs-lookup"><span data-stu-id="6971a-103">Get a member</span></span>

<span data-ttu-id="6971a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6971a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6971a-105">Use essa API para obter um membro específico (usuário ou grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="6971a-105">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="6971a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6971a-106">Permissions</span></span>
<span data-ttu-id="6971a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6971a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6971a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6971a-109">Permission type</span></span>      | <span data-ttu-id="6971a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6971a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6971a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6971a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6971a-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6971a-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6971a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6971a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6971a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6971a-114">Not supported.</span></span>    |
|<span data-ttu-id="6971a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6971a-115">Application</span></span> | <span data-ttu-id="6971a-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6971a-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6971a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6971a-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6971a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6971a-118">Request headers</span></span>
| <span data-ttu-id="6971a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6971a-119">Name</span></span>      |<span data-ttu-id="6971a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6971a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6971a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6971a-121">Authorization</span></span>  | <span data-ttu-id="6971a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6971a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6971a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6971a-124">Request body</span></span>
<span data-ttu-id="6971a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6971a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6971a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6971a-126">Response</span></span>

<span data-ttu-id="6971a-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto de [usuário](../resources/user.md) ou grupo no corpo da resposta. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="6971a-127">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6971a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6971a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6971a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6971a-129">Request</span></span>
<span data-ttu-id="6971a-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6971a-130">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="6971a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6971a-131">Response</span></span>
<span data-ttu-id="6971a-132">Aqui está um exemplo da respone.</span><span class="sxs-lookup"><span data-stu-id="6971a-132">Here is an example of the respone.</span></span> <span data-ttu-id="6971a-133">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6971a-133">Note: The response object shown here might be shortened for readability.</span></span>

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


