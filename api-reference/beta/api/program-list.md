---
title: Lista de programas
description: No Windows Azure AD para acessar o recurso de revisões, liste todos os objetos de programa.
localization_priority: Normal
ms.openlocfilehash: 9ea71e5377b7dcfe7ca6de7cfaf221e2c6dfcd98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876290"
---
# <a name="list-programs"></a><span data-ttu-id="cdfaa-103">Lista de programas</span><span class="sxs-lookup"><span data-stu-id="cdfaa-103">List programs</span></span>

> <span data-ttu-id="cdfaa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdfaa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cdfaa-106">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, liste todos os objetos de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="cdfaa-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="cdfaa-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="cdfaa-107">Permissions</span></span>
<span data-ttu-id="cdfaa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdfaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdfaa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdfaa-110">Permission type</span></span>                        | <span data-ttu-id="cdfaa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdfaa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdfaa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdfaa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdfaa-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-113"></span></span>  <span data-ttu-id="cdfaa-114">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para leitura de um programa.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="cdfaa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdfaa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdfaa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-116">Not supported.</span></span> |
|<span data-ttu-id="cdfaa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdfaa-117">Application</span></span>                            | <span data-ttu-id="cdfaa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdfaa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdfaa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="cdfaa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfaa-120">Request headers</span></span>
| <span data-ttu-id="cdfaa-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cdfaa-121">Name</span></span>         | <span data-ttu-id="cdfaa-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdfaa-122">Type</span></span>        | <span data-ttu-id="cdfaa-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdfaa-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cdfaa-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdfaa-124">Authorization</span></span> | <span data-ttu-id="cdfaa-125">string</span><span class="sxs-lookup"><span data-stu-id="cdfaa-125">string</span></span> | <span data-ttu-id="cdfaa-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-126">Bearer \{token\}.</span></span> <span data-ttu-id="cdfaa-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdfaa-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfaa-128">Request body</span></span>
<span data-ttu-id="cdfaa-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="cdfaa-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdfaa-130">Response</span></span>
<span data-ttu-id="cdfaa-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos do [programa](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-131">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdfaa-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdfaa-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdfaa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfaa-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="cdfaa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdfaa-134">Response</span></span>
><span data-ttu-id="cdfaa-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="cdfaa-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="cdfaa-137">See also</span></span>

| <span data-ttu-id="cdfaa-138">Método</span><span class="sxs-lookup"><span data-stu-id="cdfaa-138">Method</span></span>           | <span data-ttu-id="cdfaa-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cdfaa-139">Return Type</span></span>    |<span data-ttu-id="cdfaa-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdfaa-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cdfaa-141">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="cdfaa-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="cdfaa-142">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="cdfaa-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="cdfaa-143">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="cdfaa-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
