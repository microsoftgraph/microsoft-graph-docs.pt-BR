---
title: Lista businessFlowTemplates
description: No Windows Azure AD para acessar o recurso de revisões, liste todos os objetos businessFlowTemplate.
localization_priority: Normal
ms.openlocfilehash: 021a3c939c6642caf5200b5e9cc4e47b390019b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829495"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="655d4-103">Lista businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="655d4-103">List businessFlowTemplates</span></span>

> <span data-ttu-id="655d4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="655d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="655d4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="655d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="655d4-106">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, liste todos os objetos [businessFlowTemplate](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="655d4-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="655d4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="655d4-107">Permissions</span></span>
<span data-ttu-id="655d4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="655d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="655d4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="655d4-110">Permission type</span></span>                        | <span data-ttu-id="655d4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="655d4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="655d4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="655d4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="655d4-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="655d4-113"></span></span>  <span data-ttu-id="655d4-114">O usuário conectado também deve estar em uma função de diretório que permite que uma revisão de acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="655d4-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="655d4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="655d4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="655d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="655d4-116">Not supported.</span></span> |
|<span data-ttu-id="655d4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="655d4-117">Application</span></span>                            | <span data-ttu-id="655d4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="655d4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="655d4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="655d4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="655d4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="655d4-120">Request headers</span></span>
| <span data-ttu-id="655d4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="655d4-121">Name</span></span>         | <span data-ttu-id="655d4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="655d4-122">Type</span></span>        | <span data-ttu-id="655d4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="655d4-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="655d4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="655d4-124">Authorization</span></span> | <span data-ttu-id="655d4-125">string</span><span class="sxs-lookup"><span data-stu-id="655d4-125">string</span></span> | <span data-ttu-id="655d4-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="655d4-126">Bearer \{token\}.</span></span> <span data-ttu-id="655d4-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="655d4-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="655d4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="655d4-128">Request body</span></span>
<span data-ttu-id="655d4-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="655d4-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="655d4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="655d4-130">Response</span></span>
<span data-ttu-id="655d4-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [businessFlowTemplate](../resources/businessflowtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="655d4-131">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="655d4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="655d4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="655d4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="655d4-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="655d4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="655d4-134">Response</span></span>
><span data-ttu-id="655d4-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="655d4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        } 
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="655d4-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="655d4-137">See also</span></span>

| <span data-ttu-id="655d4-138">Método</span><span class="sxs-lookup"><span data-stu-id="655d4-138">Method</span></span>           | <span data-ttu-id="655d4-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="655d4-139">Return Type</span></span>    |<span data-ttu-id="655d4-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="655d4-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="655d4-141">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="655d4-141">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="655d4-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="655d4-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="655d4-143">Crie um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="655d4-143">Create a new accessReview.</span></span> |




<!-- {
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
