---
title: Lista programControls de um programa
description: No recurso de avaliações de acesso do Azure AD, liste todos os objetos de programControl, vinculados a um programa específico.
ms.openlocfilehash: 78b28851dadfa1c24bc5bc0556b1c471e7bc09e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033129"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="31ff2-103">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="31ff2-103">List programControls of a program</span></span>

> <span data-ttu-id="31ff2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="31ff2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31ff2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="31ff2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31ff2-106">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, liste todos os objetos de [programControl](../resources/programcontrol.md) , vinculados a um programa específico.</span><span class="sxs-lookup"><span data-stu-id="31ff2-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="31ff2-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="31ff2-107">Permissions</span></span>
<span data-ttu-id="31ff2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31ff2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31ff2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31ff2-110">Permission type</span></span>                        | <span data-ttu-id="31ff2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31ff2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="31ff2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31ff2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="31ff2-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="31ff2-113"></span></span>  <span data-ttu-id="31ff2-114">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para leitura de um programa.</span><span class="sxs-lookup"><span data-stu-id="31ff2-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="31ff2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31ff2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31ff2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31ff2-116">Not supported.</span></span> |
|<span data-ttu-id="31ff2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31ff2-117">Application</span></span>                            | <span data-ttu-id="31ff2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31ff2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31ff2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31ff2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="31ff2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31ff2-120">Request headers</span></span>
| <span data-ttu-id="31ff2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="31ff2-121">Name</span></span>         | <span data-ttu-id="31ff2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="31ff2-122">Type</span></span>        | <span data-ttu-id="31ff2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="31ff2-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="31ff2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="31ff2-124">Authorization</span></span> | <span data-ttu-id="31ff2-125">string</span><span class="sxs-lookup"><span data-stu-id="31ff2-125">string</span></span> | <span data-ttu-id="31ff2-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="31ff2-126">Bearer \{token\}.</span></span> <span data-ttu-id="31ff2-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31ff2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31ff2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31ff2-128">Request body</span></span>
<span data-ttu-id="31ff2-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="31ff2-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="31ff2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="31ff2-130">Response</span></span>
<span data-ttu-id="31ff2-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31ff2-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31ff2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31ff2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31ff2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31ff2-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs('673a7379-9c38-4f01-bd9d-4fda7260b807')/controls
```

##### <a name="response"></a><span data-ttu-id="31ff2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="31ff2-134">Response</span></span>
><span data-ttu-id="31ff2-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31ff2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


<!-- {
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
