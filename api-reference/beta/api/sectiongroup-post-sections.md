---
title: Criar seção
description: Crie uma nova seção no grupo de seção especificado.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 90f9958fb1be3438c878de4b83b017d0b8a15481
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977518"
---
# <a name="create-section"></a><span data-ttu-id="ef664-103">Criar seção</span><span class="sxs-lookup"><span data-stu-id="ef664-103">Create section</span></span>

> <span data-ttu-id="ef664-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef664-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef664-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef664-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef664-106">Crie uma nova [seção](../resources/section.md) no grupo de seção especificado.</span><span class="sxs-lookup"><span data-stu-id="ef664-106">Create a new [section](../resources/section.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef664-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef664-107">Permissions</span></span>
<span data-ttu-id="ef664-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef664-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef664-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef664-110">Permission type</span></span>      | <span data-ttu-id="ef664-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef664-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef664-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef664-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef664-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef664-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef664-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef664-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef664-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef664-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ef664-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef664-116">Application</span></span> | <span data-ttu-id="ef664-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef664-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef664-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef664-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="ef664-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef664-119">Request headers</span></span>
| <span data-ttu-id="ef664-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ef664-120">Name</span></span>       | <span data-ttu-id="ef664-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef664-121">Type</span></span> | <span data-ttu-id="ef664-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef664-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ef664-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef664-123">Authorization</span></span>  | <span data-ttu-id="ef664-124">string</span><span class="sxs-lookup"><span data-stu-id="ef664-124">string</span></span>  | <span data-ttu-id="ef664-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef664-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef664-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef664-127">Content-Type</span></span> | <span data-ttu-id="ef664-128">string</span><span class="sxs-lookup"><span data-stu-id="ef664-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ef664-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef664-129">Request body</span></span>
<span data-ttu-id="ef664-130">No corpo da solicitação, forneça um nome para a seção.</span><span class="sxs-lookup"><span data-stu-id="ef664-130">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="ef664-p104">Dentro do mesmo nível de hierarquia, os nomes das seções devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="ef664-p104">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="ef664-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef664-133">Response</span></span>

<span data-ttu-id="ef664-134">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [section](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef664-134">If successful, this method returns a `201 Created` response code and a [section](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef664-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef664-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef664-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef664-136">Request</span></span>
<span data-ttu-id="ef664-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef664-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="ef664-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef664-138">Response</span></span>
<span data-ttu-id="ef664-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef664-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",  
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
