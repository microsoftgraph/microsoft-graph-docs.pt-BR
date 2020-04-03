---
title: Remover um membro
description: Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3774df54f73c7e08456b3412a65378cfb51cefcf
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123339"
---
# <a name="remove-a-member"></a><span data-ttu-id="17c64-103">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="17c64-103">Remove a member</span></span>

<span data-ttu-id="17c64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17c64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17c64-105">Use esta API para remover um membro (usuário ou grupo) de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="17c64-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="17c64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="17c64-106">Permissions</span></span>
<span data-ttu-id="17c64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17c64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="17c64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17c64-109">Permission type</span></span>      | <span data-ttu-id="17c64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17c64-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17c64-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17c64-111">Delegated (work or school account)</span></span> | <span data-ttu-id="17c64-112">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="17c64-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17c64-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17c64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17c64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17c64-114">Not supported.</span></span>    |
|<span data-ttu-id="17c64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17c64-115">Application</span></span> | <span data-ttu-id="17c64-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17c64-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17c64-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17c64-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="17c64-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17c64-118">Request headers</span></span>
| <span data-ttu-id="17c64-119">Nome</span><span class="sxs-lookup"><span data-stu-id="17c64-119">Name</span></span>      |<span data-ttu-id="17c64-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="17c64-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17c64-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="17c64-121">Authorization</span></span>  | <span data-ttu-id="17c64-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17c64-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17c64-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17c64-124">Request body</span></span>
<span data-ttu-id="17c64-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17c64-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17c64-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="17c64-126">Response</span></span>

<span data-ttu-id="17c64-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17c64-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17c64-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17c64-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17c64-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17c64-130">Request</span></span>
<span data-ttu-id="17c64-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17c64-131">Here is an example of the request.</span></span> <span data-ttu-id="17c64-132">No exemplo abaixo, ID1 representa o identificador para a unidade administrativa de destino e ID2 representa o identificador exclusivo para o usuário ou grupo membro a ser removido da unidade administrativa do direcionada.</span><span class="sxs-lookup"><span data-stu-id="17c64-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="17c64-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="17c64-133">Response</span></span>
<span data-ttu-id="17c64-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17c64-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
