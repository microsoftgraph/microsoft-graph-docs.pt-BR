---
title: Excluir programa
description: No recurso de revisões do Azure AD Access, exclua um objeto Program.
localization_priority: Normal
ms.openlocfilehash: 930367e6c61d354655e73fb7ece9c8776e15f34e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546381"
---
# <a name="delete-program"></a><span data-ttu-id="753e8-103">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="753e8-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="753e8-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="753e8-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="753e8-105">Não exclua um programa que ainda esteja `programControl` vinculado a ele, essas revisões de acesso devem primeiro ser excluídas ou desvinculadas do programa e vinculadas a um programa diferente.</span><span class="sxs-lookup"><span data-stu-id="753e8-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="753e8-106">Além disso, observe que o programa padrão interno não pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="753e8-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="753e8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="753e8-107">Permissions</span></span>
<span data-ttu-id="753e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="753e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="753e8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="753e8-110">Permission type</span></span>                        | <span data-ttu-id="753e8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="753e8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="753e8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="753e8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="753e8-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="753e8-113"></span></span>  <span data-ttu-id="753e8-114">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um programa.</span><span class="sxs-lookup"><span data-stu-id="753e8-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="753e8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="753e8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="753e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="753e8-116">Not supported.</span></span> |
|<span data-ttu-id="753e8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="753e8-117">Application</span></span>                            | <span data-ttu-id="753e8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="753e8-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="753e8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="753e8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="753e8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="753e8-120">Request headers</span></span>
| <span data-ttu-id="753e8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="753e8-121">Name</span></span>         | <span data-ttu-id="753e8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="753e8-122">Type</span></span>        | <span data-ttu-id="753e8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="753e8-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="753e8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="753e8-124">Authorization</span></span> | <span data-ttu-id="753e8-125">string</span><span class="sxs-lookup"><span data-stu-id="753e8-125">string</span></span> | <span data-ttu-id="753e8-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="753e8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="753e8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="753e8-128">Request body</span></span>
<span data-ttu-id="753e8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="753e8-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="753e8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="753e8-130">Response</span></span>
<span data-ttu-id="753e8-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="753e8-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="753e8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="753e8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="753e8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="753e8-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="753e8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="753e8-135">Response</span></span>
><span data-ttu-id="753e8-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="753e8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
