---
title: Atualizar foto da equipe
description: Atualizar a foto (imagem) de uma equipe.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6c19e09713d16f8c2739b1a8398509953a19ddd0
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418332"
---
# <a name="update-team-photo"></a><span data-ttu-id="514f2-103">Atualizar foto da equipe</span><span class="sxs-lookup"><span data-stu-id="514f2-103">Update team photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="514f2-104">Atualizar a foto (imagem) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="514f2-104">Update the photo (picture) for a team.</span></span> <span data-ttu-id="514f2-105">A seguir, são apresentados os tamanhos suportados de fotos em HD no Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648 pixels.</span><span class="sxs-lookup"><span data-stu-id="514f2-105">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="514f2-106">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="514f2-106">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="514f2-107">Há um limite de 4 MB no tamanho total da solicitação.</span><span class="sxs-lookup"><span data-stu-id="514f2-107">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="514f2-108">Isso limita o tamanho da foto a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="514f2-108">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="514f2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="514f2-109">Permissions</span></span>

<span data-ttu-id="514f2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="514f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="514f2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="514f2-112">Permission type</span></span>      | <span data-ttu-id="514f2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="514f2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="514f2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="514f2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="514f2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="514f2-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="514f2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="514f2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="514f2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="514f2-117">Not supported.</span></span>    |
|<span data-ttu-id="514f2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="514f2-118">Application</span></span> | <span data-ttu-id="514f2-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="514f2-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="514f2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="514f2-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /beta/teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="514f2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="514f2-121">Request headers</span></span>

| <span data-ttu-id="514f2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="514f2-122">Header</span></span>        | <span data-ttu-id="514f2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="514f2-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="514f2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="514f2-124">Authorization</span></span> | <span data-ttu-id="514f2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="514f2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="514f2-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="514f2-127">Content-type</span></span> | <span data-ttu-id="514f2-p105">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="514f2-p105">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="514f2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="514f2-130">Request body</span></span>

<span data-ttu-id="514f2-131">No corpo da solicitação, inclua os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="514f2-131">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="514f2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="514f2-132">Response</span></span>

<span data-ttu-id="514f2-133">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="514f2-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="514f2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="514f2-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="514f2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="514f2-135">Request</span></span>

<span data-ttu-id="514f2-136">Aqui está um exemplo da solicitação para atualizar uma foto da equipe.</span><span class="sxs-lookup"><span data-stu-id="514f2-136">Here is an example of the request to update a team photo.</span></span>

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

### <a name="response"></a><span data-ttu-id="514f2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="514f2-137">Response</span></span> 

<span data-ttu-id="514f2-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="514f2-138">Here is an example of the response.</span></span>

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
