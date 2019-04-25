---
title: Listar programControls
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControl em todos os programas no locatário.
localization_priority: Normal
ms.openlocfilehash: 52361e3878445d4f739fd0cd33817d5b254ddc03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546415"
---
# <a name="list-programcontrols"></a><span data-ttu-id="d93fa-103">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="d93fa-103">List programControls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d93fa-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControl](../resources/programcontrol.md) em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="d93fa-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="d93fa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d93fa-105">Permissions</span></span>
<span data-ttu-id="d93fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93fa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d93fa-108">Permission type</span></span>                        | <span data-ttu-id="d93fa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d93fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d93fa-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d93fa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d93fa-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="d93fa-111"></span></span>  <span data-ttu-id="d93fa-112">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="d93fa-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="d93fa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d93fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d93fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d93fa-114">Not supported.</span></span> |
|<span data-ttu-id="d93fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d93fa-115">Application</span></span>                            | <span data-ttu-id="d93fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d93fa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d93fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d93fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="d93fa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d93fa-118">Request headers</span></span>
| <span data-ttu-id="d93fa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d93fa-119">Name</span></span>         | <span data-ttu-id="d93fa-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d93fa-120">Type</span></span>        | <span data-ttu-id="d93fa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d93fa-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d93fa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d93fa-122">Authorization</span></span> | <span data-ttu-id="d93fa-123">string</span><span class="sxs-lookup"><span data-stu-id="d93fa-123">string</span></span> | <span data-ttu-id="d93fa-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d93fa-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d93fa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d93fa-126">Request body</span></span>
<span data-ttu-id="d93fa-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="d93fa-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d93fa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93fa-128">Response</span></span>
<span data-ttu-id="d93fa-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d93fa-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d93fa-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d93fa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d93fa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d93fa-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="d93fa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d93fa-132">Response</span></span>
><span data-ttu-id="d93fa-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d93fa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "f6abf8ef-a05e-4788-adc9-5af909c400af",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="d93fa-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="d93fa-135">See also</span></span>

| <span data-ttu-id="d93fa-136">Método</span><span class="sxs-lookup"><span data-stu-id="d93fa-136">Method</span></span>           | <span data-ttu-id="d93fa-137">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d93fa-137">Return Type</span></span>    |<span data-ttu-id="d93fa-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d93fa-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d93fa-139">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="d93fa-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="d93fa-140">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="d93fa-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="d93fa-141">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="d93fa-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
