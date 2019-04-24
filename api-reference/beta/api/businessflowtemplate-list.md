---
title: Listar businessFlowTemplates
description: No recurso de revisões do Azure AD Access, liste todos os objetos businessFlowTemplate.
localization_priority: Normal
ms.openlocfilehash: 5b1d96330f808600c7f306ca85009bc5948a22f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461616"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="e813d-103">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="e813d-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e813d-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [businessFlowTemplate](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="e813d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e813d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e813d-105">Permissions</span></span>
<span data-ttu-id="e813d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e813d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e813d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e813d-108">Permission type</span></span>                        | <span data-ttu-id="e813d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e813d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e813d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e813d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e813d-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="e813d-111"></span></span>  <span data-ttu-id="e813d-112">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="e813d-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="e813d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e813d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e813d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e813d-114">Not supported.</span></span> |
|<span data-ttu-id="e813d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e813d-115">Application</span></span>                            | <span data-ttu-id="e813d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e813d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e813d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e813d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="e813d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e813d-118">Request headers</span></span>
| <span data-ttu-id="e813d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e813d-119">Name</span></span>         | <span data-ttu-id="e813d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e813d-120">Type</span></span>        | <span data-ttu-id="e813d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e813d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e813d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e813d-122">Authorization</span></span> | <span data-ttu-id="e813d-123">string</span><span class="sxs-lookup"><span data-stu-id="e813d-123">string</span></span> | <span data-ttu-id="e813d-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e813d-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e813d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e813d-126">Request body</span></span>
<span data-ttu-id="e813d-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="e813d-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e813d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e813d-128">Response</span></span>
<span data-ttu-id="e813d-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [businessFlowTemplate](../resources/businessflowtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e813d-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e813d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e813d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e813d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e813d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="e813d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e813d-132">Response</span></span>
><span data-ttu-id="e813d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e813d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e813d-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="e813d-135">See also</span></span>

| <span data-ttu-id="e813d-136">Método</span><span class="sxs-lookup"><span data-stu-id="e813d-136">Method</span></span>           | <span data-ttu-id="e813d-137">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e813d-137">Return Type</span></span>    |<span data-ttu-id="e813d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e813d-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e813d-139">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="e813d-139">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="e813d-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="e813d-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="e813d-141">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="e813d-141">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
