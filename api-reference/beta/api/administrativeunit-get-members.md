---
title: Obter membro
description: Use essa API para obter um determinado membro (usuário ou grupo) em uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67067d0e465aab61449a42cd833f9e6ce07fcd12
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526792"
---
# <a name="get-a-member"></a><span data-ttu-id="e0fa3-103">Obter membro</span><span class="sxs-lookup"><span data-stu-id="e0fa3-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0fa3-104">Use essa API para obter um determinado membro (usuário ou grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0fa3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0fa3-105">Permissions</span></span>
<span data-ttu-id="e0fa3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0fa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e0fa3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0fa3-108">Permission type</span></span>      | <span data-ttu-id="e0fa3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0fa3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0fa3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0fa3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0fa3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0fa3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0fa3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0fa3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0fa3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-113">Not supported.</span></span>    |
|<span data-ttu-id="e0fa3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0fa3-114">Application</span></span> | <span data-ttu-id="e0fa3-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0fa3-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0fa3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0fa3-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e0fa3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fa3-117">Request headers</span></span>
| <span data-ttu-id="e0fa3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e0fa3-118">Name</span></span>      |<span data-ttu-id="e0fa3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0fa3-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0fa3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0fa3-120">Authorization</span></span>  | <span data-ttu-id="e0fa3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0fa3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fa3-123">Request body</span></span>
<span data-ttu-id="e0fa3-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0fa3-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0fa3-125">Response</span></span>

<span data-ttu-id="e0fa3-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [usuário](../resources/user.md) ou [grupo](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0fa3-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0fa3-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0fa3-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fa3-128">Request</span></span>
<span data-ttu-id="e0fa3-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="e0fa3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0fa3-130">Response</span></span>
<span data-ttu-id="e0fa3-131">Aqui está um exemplo do respone.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-131">Here is an example of the respone.</span></span> <span data-ttu-id="e0fa3-132">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e0fa3-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0fa3-133">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
