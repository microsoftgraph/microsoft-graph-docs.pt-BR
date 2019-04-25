---
title: Excluir programControl
description: No recurso de revisões do Azure AD Access, exclua um objeto programControl.  Isso desvincula uma revisão do Access de um programa.
localization_priority: Normal
ms.openlocfilehash: 7510dfe80f758a75f190402d3ae426138e60bbed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538545"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="f70e1-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="f70e1-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f70e1-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="f70e1-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="f70e1-106">Isso desvincula uma revisão do Access de um programa.</span><span class="sxs-lookup"><span data-stu-id="f70e1-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="f70e1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f70e1-107">Permissions</span></span>
<span data-ttu-id="f70e1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f70e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f70e1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f70e1-110">Permission type</span></span>                        | <span data-ttu-id="f70e1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f70e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f70e1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f70e1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f70e1-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f70e1-113"></span></span>  <span data-ttu-id="f70e1-114">O usuário conectado também deve estar em uma função de diretório, o que permite excluir um programControl.</span><span class="sxs-lookup"><span data-stu-id="f70e1-114">The signed in user must also be in a directory role which permits them to delete a programControl.</span></span> |
|<span data-ttu-id="f70e1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f70e1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f70e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f70e1-116">Not supported.</span></span> |
|<span data-ttu-id="f70e1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f70e1-117">Application</span></span>                            | <span data-ttu-id="f70e1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f70e1-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f70e1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f70e1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="f70e1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f70e1-120">Request headers</span></span>
| <span data-ttu-id="f70e1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f70e1-121">Name</span></span>         | <span data-ttu-id="f70e1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f70e1-122">Type</span></span>        | <span data-ttu-id="f70e1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f70e1-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f70e1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f70e1-124">Authorization</span></span> | <span data-ttu-id="f70e1-125">string</span><span class="sxs-lookup"><span data-stu-id="f70e1-125">string</span></span> | <span data-ttu-id="f70e1-p105">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f70e1-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f70e1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f70e1-128">Request body</span></span>
<span data-ttu-id="f70e1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f70e1-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f70e1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f70e1-130">Response</span></span>
<span data-ttu-id="f70e1-p106">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f70e1-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f70e1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f70e1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f70e1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f70e1-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="f70e1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f70e1-135">Response</span></span>
><span data-ttu-id="f70e1-p107">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f70e1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
