---
title: Adicionar a senha do aplicativo
description: Adiciona uma senha forte a um aplicativo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 15189ee709b2b369d014f9854bcdbd4dc1b7e9be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526820"
---
# <a name="add-application-password"></a><span data-ttu-id="6d7ba-103">Adicionar a senha do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d7ba-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d7ba-104">Adiciona uma senha forte a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d7ba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d7ba-105">Permissions</span></span>
<span data-ttu-id="6d7ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d7ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d7ba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d7ba-108">Permission type</span></span>      | <span data-ttu-id="6d7ba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d7ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d7ba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d7ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d7ba-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d7ba-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d7ba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d7ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d7ba-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-113">Not supported.</span></span>    |
|<span data-ttu-id="6d7ba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d7ba-114">Application</span></span> | <span data-ttu-id="6d7ba-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d7ba-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d7ba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d7ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="6d7ba-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d7ba-117">Request headers</span></span>
| <span data-ttu-id="6d7ba-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6d7ba-118">Name</span></span>       | <span data-ttu-id="6d7ba-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d7ba-119">Type</span></span> | <span data-ttu-id="6d7ba-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d7ba-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d7ba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d7ba-121">Authorization</span></span>  | <span data-ttu-id="6d7ba-122">string</span><span class="sxs-lookup"><span data-stu-id="6d7ba-122">string</span></span>  | <span data-ttu-id="6d7ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d7ba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d7ba-125">Request body</span></span>
<span data-ttu-id="6d7ba-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d7ba-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d7ba-127">Response</span></span>

<span data-ttu-id="6d7ba-128">Se tiver êxito, este método retornará um `200 OK` objeto response de código e a senha no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="6d7ba-129">Azure AD gera uma senha forte que é retornada por meio do `secretText` propriedade.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="6d7ba-130">Não é possível recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="6d7ba-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d7ba-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d7ba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d7ba-132">Request</span></span>
<span data-ttu-id="6d7ba-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="6d7ba-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d7ba-134">Response</span></span>
<span data-ttu-id="6d7ba-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d7ba-135">Here is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/application-add-password.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
