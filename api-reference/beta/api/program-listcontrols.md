---
title: Lista programControls de um programa
description: No recurso de avaliações de acesso do Azure AD, liste todos os objetos de programControl, vinculados a um programa específico.
localization_priority: Normal
ms.openlocfilehash: 9134e9aa322446553da2e0c644a6fc8b43b0b54d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508262"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="f458e-103">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="f458e-103">List programControls of a program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f458e-104">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, liste todos os objetos de [programControl](../resources/programcontrol.md) , vinculados a um programa específico.</span><span class="sxs-lookup"><span data-stu-id="f458e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="f458e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f458e-105">Permissions</span></span>
<span data-ttu-id="f458e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f458e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f458e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f458e-108">Permission type</span></span>                        | <span data-ttu-id="f458e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f458e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f458e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f458e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f458e-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f458e-111"></span></span>  <span data-ttu-id="f458e-112">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para leitura de um programa.</span><span class="sxs-lookup"><span data-stu-id="f458e-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="f458e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f458e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f458e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f458e-114">Not supported.</span></span> |
|<span data-ttu-id="f458e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f458e-115">Application</span></span>                            | <span data-ttu-id="f458e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f458e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f458e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f458e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="f458e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f458e-118">Request headers</span></span>
| <span data-ttu-id="f458e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f458e-119">Name</span></span>         | <span data-ttu-id="f458e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f458e-120">Type</span></span>        | <span data-ttu-id="f458e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f458e-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f458e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f458e-122">Authorization</span></span> | <span data-ttu-id="f458e-123">string</span><span class="sxs-lookup"><span data-stu-id="f458e-123">string</span></span> | <span data-ttu-id="f458e-124">Token de portador</span><span class="sxs-lookup"><span data-stu-id="f458e-124">Bearer \{token\}.</span></span> <span data-ttu-id="f458e-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f458e-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f458e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f458e-126">Request body</span></span>
<span data-ttu-id="f458e-127">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="f458e-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f458e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f458e-128">Response</span></span>
<span data-ttu-id="f458e-129">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f458e-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f458e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f458e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f458e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f458e-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs('673a7379-9c38-4f01-bd9d-4fda7260b807')/controls
```

##### <a name="response"></a><span data-ttu-id="f458e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f458e-132">Response</span></span>
><span data-ttu-id="f458e-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f458e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "id": "bd68f301-e44b-4ad1-ba6d-a07314ed2e79",
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


<!--
{
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-listcontrols.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
