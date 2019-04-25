---
title: Listar programas
description: No recurso de revisões do Azure AD Access, liste todos os objetos de programa.
localization_priority: Normal
ms.openlocfilehash: 71073f2469087e92b43823e89881406fb17a666b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538596"
---
# <a name="list-programs"></a><span data-ttu-id="7834a-103">Listar programas</span><span class="sxs-lookup"><span data-stu-id="7834a-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7834a-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="7834a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7834a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7834a-105">Permissions</span></span>
<span data-ttu-id="7834a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7834a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7834a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7834a-108">Permission type</span></span>                        | <span data-ttu-id="7834a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7834a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7834a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7834a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7834a-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="7834a-111"></span></span>  <span data-ttu-id="7834a-112">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="7834a-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="7834a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7834a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7834a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7834a-114">Not supported.</span></span> |
|<span data-ttu-id="7834a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7834a-115">Application</span></span>                            | <span data-ttu-id="7834a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7834a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7834a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7834a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="7834a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7834a-118">Request headers</span></span>
| <span data-ttu-id="7834a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7834a-119">Name</span></span>         | <span data-ttu-id="7834a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7834a-120">Type</span></span>        | <span data-ttu-id="7834a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7834a-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7834a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7834a-122">Authorization</span></span> | <span data-ttu-id="7834a-123">string</span><span class="sxs-lookup"><span data-stu-id="7834a-123">string</span></span> | <span data-ttu-id="7834a-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7834a-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7834a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7834a-126">Request body</span></span>
<span data-ttu-id="7834a-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="7834a-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="7834a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7834a-128">Response</span></span>
<span data-ttu-id="7834a-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos de [programa](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7834a-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7834a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7834a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7834a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7834a-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="7834a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7834a-132">Response</span></span>
><span data-ttu-id="7834a-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7834a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="7834a-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="7834a-135">See also</span></span>

| <span data-ttu-id="7834a-136">Método</span><span class="sxs-lookup"><span data-stu-id="7834a-136">Method</span></span>           | <span data-ttu-id="7834a-137">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7834a-137">Return Type</span></span>    |<span data-ttu-id="7834a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7834a-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7834a-139">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="7834a-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="7834a-140">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="7834a-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="7834a-141">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="7834a-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
