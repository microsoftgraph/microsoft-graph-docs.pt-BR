---
title: Adicionar senha de aplicativo
description: Adiciona uma senha forte a um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 944c0a2e30a7202ad85510be84ef8b426059f4b6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289394"
---
# <a name="add-application-password"></a><span data-ttu-id="a04af-103">Adicionar senha de aplicativo</span><span class="sxs-lookup"><span data-stu-id="a04af-103">Add application password</span></span>

<span data-ttu-id="a04af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a04af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a04af-105">Adiciona uma senha forte a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a04af-105">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="a04af-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a04af-106">Permissions</span></span>
<span data-ttu-id="a04af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a04af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a04af-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a04af-109">Permission type</span></span>      | <span data-ttu-id="a04af-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a04af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a04af-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a04af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a04af-112">Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="a04af-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a04af-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a04af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a04af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a04af-114">Not supported.</span></span>    |
|<span data-ttu-id="a04af-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a04af-115">Application</span></span> | <span data-ttu-id="a04af-116">Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a04af-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a04af-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a04af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="a04af-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a04af-118">Request headers</span></span>
| <span data-ttu-id="a04af-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a04af-119">Name</span></span>       | <span data-ttu-id="a04af-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a04af-120">Type</span></span> | <span data-ttu-id="a04af-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a04af-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a04af-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a04af-122">Authorization</span></span>  | <span data-ttu-id="a04af-123">string</span><span class="sxs-lookup"><span data-stu-id="a04af-123">string</span></span>  | <span data-ttu-id="a04af-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a04af-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a04af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a04af-126">Request body</span></span>
<span data-ttu-id="a04af-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a04af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a04af-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a04af-128">Response</span></span>

<span data-ttu-id="a04af-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto password no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a04af-129">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="a04af-130">O Azure AD gera uma senha forte que é retornada por meio da `secretText` propriedade.</span><span class="sxs-lookup"><span data-stu-id="a04af-130">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="a04af-131">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="a04af-131">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="a04af-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a04af-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a04af-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a04af-133">Request</span></span>
<span data-ttu-id="a04af-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a04af-134">The following is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="a04af-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a04af-135">Response</span></span>
<span data-ttu-id="a04af-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a04af-136">The following is an example of the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "customKeyIdentifier": "Binary",
    "endDateTime": "String (timestamp)",
    "keyId": "String (identifier)",
    "startDateTime": "String (timestamp)",
    "secretText": "String",
    "hint": "String"
}
```
