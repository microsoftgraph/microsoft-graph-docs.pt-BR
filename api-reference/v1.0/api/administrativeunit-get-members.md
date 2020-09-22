---
title: Obter um membro
description: Use essa API para obter um membro específico (usuário ou grupo) em uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6cf700fad752071603586d29cc892a28763616a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020204"
---
# <a name="get-a-member"></a><span data-ttu-id="59160-103">Obter um membro</span><span class="sxs-lookup"><span data-stu-id="59160-103">Get a member</span></span>

<span data-ttu-id="59160-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59160-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59160-105">Use essa API para obter um membro específico (usuário ou grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="59160-105">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="59160-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59160-106">Permissions</span></span>
<span data-ttu-id="59160-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59160-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="59160-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59160-109">Permission type</span></span>      | <span data-ttu-id="59160-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59160-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59160-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59160-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59160-112">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="59160-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="59160-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59160-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59160-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59160-114">Not supported.</span></span>    |
|<span data-ttu-id="59160-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59160-115">Application</span></span> | <span data-ttu-id="59160-116">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="59160-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59160-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59160-117">HTTP request</span></span>

```http
GET /directory/administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="59160-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59160-118">Request headers</span></span>
| <span data-ttu-id="59160-119">Nome</span><span class="sxs-lookup"><span data-stu-id="59160-119">Name</span></span>      |<span data-ttu-id="59160-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="59160-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59160-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="59160-121">Authorization</span></span>  | <span data-ttu-id="59160-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59160-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59160-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59160-124">Request body</span></span>
<span data-ttu-id="59160-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59160-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59160-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="59160-126">Response</span></span>

<span data-ttu-id="59160-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [User](../resources/user.md) ou [Group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59160-127">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59160-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59160-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59160-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59160-129">Request</span></span>
<span data-ttu-id="59160-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59160-130">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="59160-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="59160-131">Response</span></span>
<span data-ttu-id="59160-132">Veja um exemplo de Respone.</span><span class="sxs-lookup"><span data-stu-id="59160-132">Here is an example of the respone.</span></span> <span data-ttu-id="59160-133">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="59160-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="59160-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59160-134">All of the properties will be returned from an actual call.</span></span>

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
