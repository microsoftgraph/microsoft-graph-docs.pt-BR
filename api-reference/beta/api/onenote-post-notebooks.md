---
title: Criar bloco de anotações
description: Crie um novo bloco de anotações do OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 8ad8f2f68989796c2c041fdd758017044f0c73e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826583"
---
# <a name="create-notebook"></a><span data-ttu-id="6f1c9-103">Criar bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="6f1c9-103">Create notebook</span></span>

> <span data-ttu-id="6f1c9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f1c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f1c9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f1c9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f1c9-106">Crie um novo [bloco de anotações](../resources/notebook.md) do OneNote.</span><span class="sxs-lookup"><span data-stu-id="6f1c9-106">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6f1c9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f1c9-107">Permissions</span></span>
<span data-ttu-id="6f1c9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f1c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f1c9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f1c9-110">Permission type</span></span>      | <span data-ttu-id="6f1c9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f1c9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f1c9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f1c9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6f1c9-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f1c9-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f1c9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f1c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f1c9-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f1c9-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6f1c9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f1c9-116">Application</span></span> | <span data-ttu-id="6f1c9-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f1c9-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f1c9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f1c9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="6f1c9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f1c9-119">Request headers</span></span>
| <span data-ttu-id="6f1c9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6f1c9-120">Name</span></span>       | <span data-ttu-id="6f1c9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f1c9-121">Type</span></span> | <span data-ttu-id="6f1c9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f1c9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f1c9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f1c9-123">Authorization</span></span>  | <span data-ttu-id="6f1c9-124">string</span><span class="sxs-lookup"><span data-stu-id="6f1c9-124">string</span></span>  | <span data-ttu-id="6f1c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f1c9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6f1c9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f1c9-127">Content-Type</span></span> | <span data-ttu-id="6f1c9-128">string</span><span class="sxs-lookup"><span data-stu-id="6f1c9-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6f1c9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f1c9-129">Request body</span></span>
<span data-ttu-id="6f1c9-130">No corpo da solicitação, forneça um nome para o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="6f1c9-130">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="6f1c9-p104">Os nomes dos blocos de anotações devem ser exclusivos. O nome não pode conter mais de 128 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="6f1c9-p104">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="6f1c9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f1c9-133">Response</span></span>

<span data-ttu-id="6f1c9-134">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f1c9-134">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f1c9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f1c9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f1c9-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f1c9-136">Request</span></span>
<span data-ttu-id="6f1c9-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f1c9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="6f1c9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f1c9-138">Response</span></span>
<span data-ttu-id="6f1c9-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f1c9-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
