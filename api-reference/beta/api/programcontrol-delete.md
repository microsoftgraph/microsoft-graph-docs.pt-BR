---
title: Excluir programControl
description: No Windows Azure AD para acessar o recurso de revisões, excluir um objeto programControl.  Isso desvincula uma revisão de acesso de um programa.
ms.openlocfilehash: a7f21cd4c18ecda2ce15a6dd76d87322f75e4af0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035671"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="5a62c-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="5a62c-104">Delete programControl</span></span>

> <span data-ttu-id="5a62c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a62c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a62c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a62c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a62c-107">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, exclua um objeto de [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="5a62c-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="5a62c-108">Isso desvincula uma revisão de acesso de um programa.</span><span class="sxs-lookup"><span data-stu-id="5a62c-108">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a62c-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="5a62c-109">Permissions</span></span>
<span data-ttu-id="5a62c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a62c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a62c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a62c-112">Permission type</span></span>                        | <span data-ttu-id="5a62c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a62c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a62c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a62c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a62c-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="5a62c-115"></span></span>  <span data-ttu-id="5a62c-116">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para excluir um programControl.</span><span class="sxs-lookup"><span data-stu-id="5a62c-116">The signed in user must also be in a directory role which permits them to delete a programControl.</span></span> |
|<span data-ttu-id="5a62c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a62c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a62c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a62c-118">Not supported.</span></span> |
|<span data-ttu-id="5a62c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a62c-119">Application</span></span>                            | <span data-ttu-id="5a62c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a62c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a62c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a62c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="5a62c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a62c-122">Request headers</span></span>
| <span data-ttu-id="5a62c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5a62c-123">Name</span></span>         | <span data-ttu-id="5a62c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a62c-124">Type</span></span>        | <span data-ttu-id="5a62c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a62c-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5a62c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a62c-126">Authorization</span></span> | <span data-ttu-id="5a62c-127">string</span><span class="sxs-lookup"><span data-stu-id="5a62c-127">string</span></span> | <span data-ttu-id="5a62c-128">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="5a62c-128">Bearer \{token\}.</span></span> <span data-ttu-id="5a62c-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a62c-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a62c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a62c-130">Request body</span></span>
<span data-ttu-id="5a62c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a62c-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5a62c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a62c-132">Response</span></span>
<span data-ttu-id="5a62c-p107">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a62c-p107">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a62c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a62c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a62c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a62c-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="5a62c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a62c-137">Response</span></span>
><span data-ttu-id="5a62c-p108">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a62c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
