---
title: Lista programControls
description: No recurso de avaliações de acesso do Azure AD, liste todos os objetos de programControl, em todos os programas no inquilino.
localization_priority: Normal
ms.openlocfilehash: bc56fd5013bcf0013007b9d4264ab89eca02d43b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843950"
---
# <a name="list-programcontrols"></a><span data-ttu-id="1251e-103">Lista programControls</span><span class="sxs-lookup"><span data-stu-id="1251e-103">List programControls</span></span>

> <span data-ttu-id="1251e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1251e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1251e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1251e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1251e-106">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, liste todos os objetos de [programControl](../resources/programcontrol.md) , em todos os programas no inquilino.</span><span class="sxs-lookup"><span data-stu-id="1251e-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="1251e-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1251e-107">Permissions</span></span>
<span data-ttu-id="1251e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1251e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1251e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1251e-110">Permission type</span></span>                        | <span data-ttu-id="1251e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1251e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1251e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1251e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1251e-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="1251e-113"></span></span>  <span data-ttu-id="1251e-114">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para leitura de um programa.</span><span class="sxs-lookup"><span data-stu-id="1251e-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="1251e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1251e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1251e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1251e-116">Not supported.</span></span> |
|<span data-ttu-id="1251e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1251e-117">Application</span></span>                            | <span data-ttu-id="1251e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1251e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1251e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1251e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="1251e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1251e-120">Request headers</span></span>
| <span data-ttu-id="1251e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1251e-121">Name</span></span>         | <span data-ttu-id="1251e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1251e-122">Type</span></span>        | <span data-ttu-id="1251e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1251e-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1251e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1251e-124">Authorization</span></span> | <span data-ttu-id="1251e-125">string</span><span class="sxs-lookup"><span data-stu-id="1251e-125">string</span></span> | <span data-ttu-id="1251e-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="1251e-126">Bearer \{token\}.</span></span> <span data-ttu-id="1251e-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1251e-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1251e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1251e-128">Request body</span></span>
<span data-ttu-id="1251e-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="1251e-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="1251e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1251e-130">Response</span></span>
<span data-ttu-id="1251e-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1251e-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1251e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1251e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1251e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1251e-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="1251e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1251e-134">Response</span></span>
><span data-ttu-id="1251e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1251e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1251e-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="1251e-137">See also</span></span>

| <span data-ttu-id="1251e-138">Método</span><span class="sxs-lookup"><span data-stu-id="1251e-138">Method</span></span>           | <span data-ttu-id="1251e-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1251e-139">Return Type</span></span>    |<span data-ttu-id="1251e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="1251e-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1251e-141">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="1251e-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="1251e-142">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="1251e-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="1251e-143">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="1251e-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
