---
title: Excluir programa
description: No Windows Azure AD para acessar o recurso de revisões, excluir um objeto de programa.
ms.openlocfilehash: c09dcc36bfc4fbf279e7b6c49ea24bba9153c071
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038684"
---
# <a name="delete-program"></a><span data-ttu-id="de8ba-103">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="de8ba-103">Delete program</span></span>

> <span data-ttu-id="de8ba-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="de8ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de8ba-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="de8ba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de8ba-106">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, exclua um objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="de8ba-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="de8ba-107">Não exclua um programa que ainda tem `programControl` vinculadas a ela, as avaliações de acesso devem primeiro ser excluídas ou desligadas a partir do programa e vinculadas a um programa diferente.</span><span class="sxs-lookup"><span data-stu-id="de8ba-107">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="de8ba-108">Além disso, observe que o programa internos padrão não pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="de8ba-108">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="de8ba-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="de8ba-109">Permissions</span></span>
<span data-ttu-id="de8ba-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de8ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de8ba-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de8ba-112">Permission type</span></span>                        | <span data-ttu-id="de8ba-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de8ba-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="de8ba-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de8ba-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="de8ba-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="de8ba-115"></span></span>  <span data-ttu-id="de8ba-116">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para criar um programa.</span><span class="sxs-lookup"><span data-stu-id="de8ba-116">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="de8ba-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de8ba-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de8ba-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de8ba-118">Not supported.</span></span> |
|<span data-ttu-id="de8ba-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de8ba-119">Application</span></span>                            | <span data-ttu-id="de8ba-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de8ba-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de8ba-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de8ba-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="de8ba-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de8ba-122">Request headers</span></span>
| <span data-ttu-id="de8ba-123">Nome</span><span class="sxs-lookup"><span data-stu-id="de8ba-123">Name</span></span>         | <span data-ttu-id="de8ba-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="de8ba-124">Type</span></span>        | <span data-ttu-id="de8ba-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="de8ba-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="de8ba-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="de8ba-126">Authorization</span></span> | <span data-ttu-id="de8ba-127">string</span><span class="sxs-lookup"><span data-stu-id="de8ba-127">string</span></span> | <span data-ttu-id="de8ba-128">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="de8ba-128">Bearer \{token\}.</span></span> <span data-ttu-id="de8ba-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de8ba-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de8ba-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de8ba-130">Request body</span></span>
<span data-ttu-id="de8ba-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de8ba-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="de8ba-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="de8ba-132">Response</span></span>
<span data-ttu-id="de8ba-p106">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de8ba-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de8ba-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de8ba-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de8ba-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de8ba-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="de8ba-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="de8ba-137">Response</span></span>
><span data-ttu-id="de8ba-p107">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de8ba-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
