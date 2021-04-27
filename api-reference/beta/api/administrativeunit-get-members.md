---
title: Obter um membro
description: Use essa API para obter um membro específico (usuário ou grupo) em uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2cd676d8509a082cabbf896ff68300488f6dc352
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048271"
---
# <a name="get-a-member"></a><span data-ttu-id="ead07-103">Obter um membro</span><span class="sxs-lookup"><span data-stu-id="ead07-103">Get a member</span></span>

<span data-ttu-id="ead07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ead07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ead07-105">Use essa API para obter um membro específico (usuário ou grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="ead07-105">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="ead07-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ead07-106">Permissions</span></span>
<span data-ttu-id="ead07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ead07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ead07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ead07-109">Permission type</span></span>      | <span data-ttu-id="ead07-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ead07-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ead07-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ead07-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ead07-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ead07-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ead07-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ead07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ead07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ead07-114">Not supported.</span></span>    |
|<span data-ttu-id="ead07-115">Application</span><span class="sxs-lookup"><span data-stu-id="ead07-115">Application</span></span> | <span data-ttu-id="ead07-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ead07-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ead07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ead07-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ead07-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ead07-118">Request headers</span></span>
| <span data-ttu-id="ead07-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ead07-119">Name</span></span>      |<span data-ttu-id="ead07-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ead07-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ead07-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ead07-121">Authorization</span></span>  | <span data-ttu-id="ead07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ead07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ead07-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ead07-124">Request body</span></span>
<span data-ttu-id="ead07-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ead07-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ead07-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ead07-126">Response</span></span>

<span data-ttu-id="ead07-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto de [usuário](../resources/user.md) ou grupo no corpo da resposta. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="ead07-127">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ead07-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ead07-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ead07-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ead07-129">Request</span></span>
<span data-ttu-id="ead07-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ead07-130">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="ead07-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ead07-131">Response</span></span>
<span data-ttu-id="ead07-132">Aqui está um exemplo da respone.</span><span class="sxs-lookup"><span data-stu-id="ead07-132">Here is an example of the respone.</span></span> <span data-ttu-id="ead07-133">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ead07-133">Note: The response object shown here might be shortened for readability.</span></span>

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


