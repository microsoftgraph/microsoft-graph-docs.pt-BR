---
title: Listar programControls de um programa
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControl vinculados a um programa específico.
localization_priority: Normal
ms.openlocfilehash: 787199b4c254411166d30e960024923cfe1d279f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331948"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="816eb-103">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="816eb-103">List programControls of a program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="816eb-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControl](../resources/programcontrol.md) vinculados a um programa específico.</span><span class="sxs-lookup"><span data-stu-id="816eb-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="816eb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="816eb-105">Permissions</span></span>
<span data-ttu-id="816eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="816eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="816eb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="816eb-108">Permission type</span></span>                        | <span data-ttu-id="816eb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="816eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="816eb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="816eb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="816eb-111">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="816eb-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="816eb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="816eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="816eb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="816eb-113">Not supported.</span></span> |
|<span data-ttu-id="816eb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="816eb-114">Application</span></span>                            | <span data-ttu-id="816eb-115">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="816eb-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="816eb-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="816eb-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="816eb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="816eb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="816eb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="816eb-118">Request headers</span></span>
| <span data-ttu-id="816eb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="816eb-119">Name</span></span>         | <span data-ttu-id="816eb-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="816eb-120">Type</span></span>        | <span data-ttu-id="816eb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="816eb-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="816eb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="816eb-122">Authorization</span></span> | <span data-ttu-id="816eb-123">string</span><span class="sxs-lookup"><span data-stu-id="816eb-123">string</span></span> | <span data-ttu-id="816eb-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="816eb-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="816eb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="816eb-126">Request body</span></span>
<span data-ttu-id="816eb-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="816eb-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="816eb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="816eb-128">Response</span></span>
<span data-ttu-id="816eb-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="816eb-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="816eb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="816eb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="816eb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="816eb-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```

##### <a name="response"></a><span data-ttu-id="816eb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="816eb-132">Response</span></span>
><span data-ttu-id="816eb-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="816eb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
