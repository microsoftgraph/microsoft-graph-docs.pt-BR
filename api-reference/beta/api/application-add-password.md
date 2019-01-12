---
title: Adicionar a senha do aplicativo
description: Adiciona uma senha forte a um aplicativo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 565fbab9ff2cde34bcccbe760692df9d3c0d1a14
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966759"
---
# <a name="add-application-password"></a><span data-ttu-id="47a55-103">Adicionar a senha do aplicativo</span><span class="sxs-lookup"><span data-stu-id="47a55-103">Add application password</span></span>

> <span data-ttu-id="47a55-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="47a55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47a55-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="47a55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47a55-106">Adiciona uma senha forte a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47a55-106">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="47a55-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="47a55-107">Permissions</span></span>
<span data-ttu-id="47a55-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47a55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47a55-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47a55-110">Permission type</span></span>      | <span data-ttu-id="47a55-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47a55-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47a55-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47a55-112">Delegated (work or school account)</span></span> | <span data-ttu-id="47a55-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47a55-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47a55-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47a55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47a55-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47a55-115">Not supported.</span></span>    |
|<span data-ttu-id="47a55-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47a55-116">Application</span></span> | <span data-ttu-id="47a55-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="47a55-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47a55-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47a55-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="47a55-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47a55-119">Request headers</span></span>
| <span data-ttu-id="47a55-120">Nome</span><span class="sxs-lookup"><span data-stu-id="47a55-120">Name</span></span>       | <span data-ttu-id="47a55-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="47a55-121">Type</span></span> | <span data-ttu-id="47a55-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="47a55-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="47a55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47a55-123">Authorization</span></span>  | <span data-ttu-id="47a55-124">string</span><span class="sxs-lookup"><span data-stu-id="47a55-124">string</span></span>  | <span data-ttu-id="47a55-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47a55-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47a55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47a55-127">Request body</span></span>
<span data-ttu-id="47a55-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47a55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47a55-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="47a55-129">Response</span></span>

<span data-ttu-id="47a55-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e a senha no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47a55-130">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="47a55-131">Azure AD gera uma senha forte que é retornada por meio do `secretText` propriedade.</span><span class="sxs-lookup"><span data-stu-id="47a55-131">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="47a55-132">Não é possível recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="47a55-132">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="47a55-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47a55-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47a55-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47a55-134">Request</span></span>
<span data-ttu-id="47a55-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47a55-135">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="47a55-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="47a55-136">Response</span></span>
<span data-ttu-id="47a55-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47a55-137">Here is an example of the response.</span></span>

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
