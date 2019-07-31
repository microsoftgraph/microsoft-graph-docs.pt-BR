---
title: Adicionar senha de aplicativo
description: Adiciona uma senha forte a um aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fcd4701b2c9161582b9bd951f35bf0c8ba09821
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945561"
---
# <a name="add-application-password"></a><span data-ttu-id="62c57-103">Adicionar senha de aplicativo</span><span class="sxs-lookup"><span data-stu-id="62c57-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62c57-104">Adiciona uma senha forte a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62c57-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="62c57-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="62c57-105">Permissions</span></span>
<span data-ttu-id="62c57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62c57-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62c57-108">Permission type</span></span>      | <span data-ttu-id="62c57-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62c57-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62c57-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62c57-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62c57-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62c57-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62c57-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62c57-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62c57-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62c57-113">Not supported.</span></span>    |
|<span data-ttu-id="62c57-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62c57-114">Application</span></span> | <span data-ttu-id="62c57-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="62c57-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62c57-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62c57-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="62c57-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62c57-117">Request headers</span></span>
| <span data-ttu-id="62c57-118">Nome</span><span class="sxs-lookup"><span data-stu-id="62c57-118">Name</span></span>       | <span data-ttu-id="62c57-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="62c57-119">Type</span></span> | <span data-ttu-id="62c57-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="62c57-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="62c57-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="62c57-121">Authorization</span></span>  | <span data-ttu-id="62c57-122">string</span><span class="sxs-lookup"><span data-stu-id="62c57-122">string</span></span>  | <span data-ttu-id="62c57-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62c57-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62c57-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62c57-125">Request body</span></span>
<span data-ttu-id="62c57-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62c57-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62c57-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="62c57-127">Response</span></span>

<span data-ttu-id="62c57-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto password no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62c57-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="62c57-129">O Azure AD gera uma senha forte que é retornada por `secretText` meio da propriedade.</span><span class="sxs-lookup"><span data-stu-id="62c57-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="62c57-130">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="62c57-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="62c57-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62c57-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62c57-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62c57-132">Request</span></span>
<span data-ttu-id="62c57-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62c57-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="62c57-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="62c57-134">Response</span></span>
<span data-ttu-id="62c57-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62c57-135">Here is an example of the response.</span></span>

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
