---
title: Adicionar a senha do aplicativo
description: Adiciona uma senha forte a um aplicativo.
author: lleonard-msft
ms.openlocfilehash: 88aa499cd478511aacba94c0d28c96592c79a5d5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348738"
---
# <a name="add-application-password"></a><span data-ttu-id="67b68-103">Adicionar a senha do aplicativo</span><span class="sxs-lookup"><span data-stu-id="67b68-103">Add application password</span></span>

> <span data-ttu-id="67b68-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="67b68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67b68-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67b68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67b68-106">Adiciona uma senha forte a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="67b68-106">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="67b68-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="67b68-107">Permissions</span></span>
<span data-ttu-id="67b68-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67b68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67b68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67b68-110">Permission type</span></span>      | <span data-ttu-id="67b68-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67b68-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67b68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67b68-112">Delegated (work or school account)</span></span> | <span data-ttu-id="67b68-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67b68-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67b68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67b68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67b68-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67b68-115">Not supported.</span></span>    |
|<span data-ttu-id="67b68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67b68-116">Application</span></span> | <span data-ttu-id="67b68-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="67b68-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67b68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67b68-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="67b68-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67b68-119">Request headers</span></span>
| <span data-ttu-id="67b68-120">Nome</span><span class="sxs-lookup"><span data-stu-id="67b68-120">Name</span></span>       | <span data-ttu-id="67b68-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="67b68-121">Type</span></span> | <span data-ttu-id="67b68-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="67b68-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="67b68-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67b68-123">Authorization</span></span>  | <span data-ttu-id="67b68-124">string</span><span class="sxs-lookup"><span data-stu-id="67b68-124">string</span></span>  | <span data-ttu-id="67b68-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67b68-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67b68-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67b68-127">Request body</span></span>
<span data-ttu-id="67b68-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67b68-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67b68-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67b68-129">Response</span></span>

<span data-ttu-id="67b68-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e a senha no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67b68-130">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="67b68-131">Azure AD gera uma senha forte que é retornada por meio do `secretText` propriedade.</span><span class="sxs-lookup"><span data-stu-id="67b68-131">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="67b68-132">Não é possível recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="67b68-132">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="67b68-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67b68-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67b68-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67b68-134">Request</span></span>
<span data-ttu-id="67b68-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67b68-135">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="67b68-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="67b68-136">Response</span></span>
<span data-ttu-id="67b68-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67b68-137">Here is an example of the response.</span></span>

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
