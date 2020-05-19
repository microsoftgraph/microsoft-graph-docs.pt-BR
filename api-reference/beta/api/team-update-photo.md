---
title: Atualizar foto da equipe
description: Atualizar a foto (imagem) de uma equipe.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a33220682e2df2fb084944cfb8474c592e7649d7
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290087"
---
# <a name="update-team-photo"></a><span data-ttu-id="0c16d-103">Atualizar foto da equipe</span><span class="sxs-lookup"><span data-stu-id="0c16d-103">Update team photo</span></span>

<span data-ttu-id="0c16d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c16d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c16d-105">Atualizar a foto (imagem) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="0c16d-105">Update the photo (picture) for a team.</span></span> <span data-ttu-id="0c16d-106">A seguir, são apresentados os tamanhos suportados de fotos em HD no Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648 pixels.</span><span class="sxs-lookup"><span data-stu-id="0c16d-106">The following are the supported sizes of HD photos in Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="0c16d-107">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0c16d-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="0c16d-108">Há um limite de 4 MB no tamanho total da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c16d-108">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="0c16d-109">Isso limita o tamanho da foto a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="0c16d-109">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c16d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c16d-110">Permissions</span></span>

<span data-ttu-id="0c16d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c16d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c16d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c16d-113">Permission type</span></span>      | <span data-ttu-id="0c16d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c16d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c16d-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c16d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0c16d-116">TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0c16d-116">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="0c16d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c16d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c16d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c16d-118">Not supported.</span></span>    |
|<span data-ttu-id="0c16d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c16d-119">Application</span></span> | <span data-ttu-id="0c16d-120">TeamSettings. Edit. Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0c16d-120">TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c16d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c16d-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="0c16d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c16d-122">Request headers</span></span>

| <span data-ttu-id="0c16d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c16d-123">Header</span></span>        | <span data-ttu-id="0c16d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0c16d-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="0c16d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c16d-125">Authorization</span></span> | <span data-ttu-id="0c16d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c16d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c16d-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="0c16d-128">Content-type</span></span> | <span data-ttu-id="0c16d-p105">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c16d-p105">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c16d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c16d-131">Request body</span></span>

<span data-ttu-id="0c16d-132">No corpo da solicitação, inclua os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="0c16d-132">In the request body, include the binary data of the photo.</span></span>

## <a name="response"></a><span data-ttu-id="0c16d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c16d-133">Response</span></span>

<span data-ttu-id="0c16d-134">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="0c16d-134">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c16d-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c16d-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c16d-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c16d-136">Request</span></span>

<span data-ttu-id="0c16d-137">Aqui está um exemplo da solicitação para atualizar uma foto da equipe.</span><span class="sxs-lookup"><span data-stu-id="0c16d-137">Here is an example of the request to update a team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{id}/photo
Content-type: image/jpeg

{
  <Binary data for the image>
}
```

### <a name="response"></a><span data-ttu-id="0c16d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c16d-138">Response</span></span> 

<span data-ttu-id="0c16d-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c16d-139">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
