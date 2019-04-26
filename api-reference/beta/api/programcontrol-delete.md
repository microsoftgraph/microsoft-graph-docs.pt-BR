---
title: Excluir programControl
description: No recurso de revisões do Azure AD Access, exclua um objeto programControl.  Isso desvincula uma revisão do Access de um programa.
localization_priority: Normal
ms.openlocfilehash: c0c0e3b9323777db946e562d9c6ea6aa3b81e92f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337253"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="16b94-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="16b94-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16b94-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="16b94-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="16b94-106">Isso desvincula uma revisão do Access de um programa.</span><span class="sxs-lookup"><span data-stu-id="16b94-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="16b94-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16b94-107">Permissions</span></span>
<span data-ttu-id="16b94-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16b94-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16b94-110">Permission type</span></span>                        | <span data-ttu-id="16b94-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16b94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="16b94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16b94-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="16b94-113">ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="16b94-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="16b94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16b94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16b94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16b94-115">Not supported.</span></span> |
|<span data-ttu-id="16b94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16b94-116">Application</span></span>                            | <span data-ttu-id="16b94-117">ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="16b94-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="16b94-118">O usuário conectado também deve estar em uma função de diretório que permite excluir um `programControl`.</span><span class="sxs-lookup"><span data-stu-id="16b94-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="16b94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16b94-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="16b94-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16b94-120">Request headers</span></span>
| <span data-ttu-id="16b94-121">Nome</span><span class="sxs-lookup"><span data-stu-id="16b94-121">Name</span></span>         | <span data-ttu-id="16b94-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="16b94-122">Type</span></span>        | <span data-ttu-id="16b94-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="16b94-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="16b94-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="16b94-124">Authorization</span></span> | <span data-ttu-id="16b94-125">string</span><span class="sxs-lookup"><span data-stu-id="16b94-125">string</span></span> | <span data-ttu-id="16b94-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16b94-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16b94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16b94-128">Request body</span></span>
<span data-ttu-id="16b94-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16b94-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="16b94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b94-130">Response</span></span>
<span data-ttu-id="16b94-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16b94-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16b94-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16b94-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16b94-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16b94-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
##### <a name="response"></a><span data-ttu-id="16b94-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b94-135">Response</span></span>
><span data-ttu-id="16b94-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16b94-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
