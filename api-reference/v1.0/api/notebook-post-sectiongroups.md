---
title: Criar sectionGroup
description: Cria um novo grupo de seção no bloco de anotações especificado.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 31a0f13c30682e491016b6dce4675b8159b8d897
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562136"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="e8eb5-103">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="e8eb5-103">Create sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8eb5-104">Cria um novo [grupo de seção](../resources/sectiongroup.md) no bloco de anotações especificado.</span><span class="sxs-lookup"><span data-stu-id="e8eb5-104">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8eb5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8eb5-105">Permissions</span></span>
<span data-ttu-id="e8eb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8eb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8eb5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8eb5-108">Permission type</span></span>      | <span data-ttu-id="e8eb5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8eb5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8eb5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8eb5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8eb5-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8eb5-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8eb5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8eb5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8eb5-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8eb5-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e8eb5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8eb5-114">Application</span></span> | <span data-ttu-id="e8eb5-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8eb5-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8eb5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8eb5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="e8eb5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8eb5-117">Request headers</span></span>
| <span data-ttu-id="e8eb5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e8eb5-118">Name</span></span>       | <span data-ttu-id="e8eb5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8eb5-119">Type</span></span> | <span data-ttu-id="e8eb5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8eb5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8eb5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8eb5-121">Authorization</span></span>  | <span data-ttu-id="e8eb5-122">string</span><span class="sxs-lookup"><span data-stu-id="e8eb5-122">string</span></span>  | <span data-ttu-id="e8eb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8eb5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8eb5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8eb5-125">Content-Type</span></span> | <span data-ttu-id="e8eb5-126">string</span><span class="sxs-lookup"><span data-stu-id="e8eb5-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e8eb5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8eb5-127">Request body</span></span>
<span data-ttu-id="e8eb5-128">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="e8eb5-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="e8eb5-p103">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="e8eb5-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="e8eb5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8eb5-131">Response</span></span>

<span data-ttu-id="e8eb5-132">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto de objeto de [seção](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8eb5-132">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8eb5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8eb5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8eb5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8eb5-134">Request</span></span>
<span data-ttu-id="e8eb5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8eb5-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```

##### <a name="response"></a><span data-ttu-id="e8eb5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8eb5-136">Response</span></span>
<span data-ttu-id="e8eb5-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8eb5-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
