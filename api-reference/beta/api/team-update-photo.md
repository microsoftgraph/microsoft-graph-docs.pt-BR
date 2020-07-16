---
title: Atualizar foto da equipe
description: Atualizar a foto (imagem) de uma equipe.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 22fdca19b657bdf439f356fb61e4f805f45b4f4b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896123"
---
# <a name="update-team-photo"></a><span data-ttu-id="d698b-103">Atualizar foto da equipe</span><span class="sxs-lookup"><span data-stu-id="d698b-103">Update team photo</span></span>

<span data-ttu-id="d698b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d698b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d698b-105">Atualizar a foto (imagem) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d698b-105">Update the photo (picture) for a team.</span></span> <span data-ttu-id="d698b-106">Estes são os tamanhos de fotos de HD compatíveis no Microsoft 365:48x48, 64x64, 96x96, 120x120, 240x240, 360X360, 432x432, 504x504 e 648x648 pixels.</span><span class="sxs-lookup"><span data-stu-id="d698b-106">The following are the supported sizes of HD photos in Microsoft 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="d698b-107">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d698b-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="d698b-108">Há um limite de 4 MB no tamanho total da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d698b-108">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="d698b-109">Isso limita o tamanho da foto a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="d698b-109">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="d698b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d698b-110">Permissions</span></span>

<span data-ttu-id="d698b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d698b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d698b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d698b-113">Permission type</span></span>      | <span data-ttu-id="d698b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d698b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d698b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d698b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d698b-116">TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d698b-116">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d698b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d698b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d698b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d698b-118">Not supported.</span></span>    |
|<span data-ttu-id="d698b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d698b-119">Application</span></span> | <span data-ttu-id="d698b-120">TeamSettings. Edit. Group \*, TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d698b-120">TeamSettings.Edit.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d698b-121">**Observação**: as permissões marcadas com \* usam o [consentimento específico do recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d698b-121">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="d698b-122">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d698b-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d698b-123">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d698b-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d698b-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d698b-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="d698b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d698b-125">Request headers</span></span>

| <span data-ttu-id="d698b-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d698b-126">Header</span></span>        | <span data-ttu-id="d698b-127">Valor</span><span class="sxs-lookup"><span data-stu-id="d698b-127">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="d698b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d698b-128">Authorization</span></span> | <span data-ttu-id="d698b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d698b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d698b-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="d698b-131">Content-type</span></span> | <span data-ttu-id="d698b-p106">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d698b-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d698b-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d698b-134">Request body</span></span>

<span data-ttu-id="d698b-135">No corpo da solicitação, inclua os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="d698b-135">In the request body, include the binary data of the photo.</span></span>

## <a name="response"></a><span data-ttu-id="d698b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d698b-136">Response</span></span>

<span data-ttu-id="d698b-137">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d698b-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d698b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d698b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d698b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d698b-139">Request</span></span>

<span data-ttu-id="d698b-140">Aqui está um exemplo da solicitação para atualizar uma foto da equipe.</span><span class="sxs-lookup"><span data-stu-id="d698b-140">Here is an example of the request to update a team photo.</span></span>

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

### <a name="response"></a><span data-ttu-id="d698b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d698b-141">Response</span></span> 

<span data-ttu-id="d698b-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d698b-142">Here is an example of the response.</span></span>

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
