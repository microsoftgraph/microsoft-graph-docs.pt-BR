---
title: Adicionar o aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
ms.openlocfilehash: ec03c0f8744bd2f1dd5cf5e2a7e84c9b59a7c6ce
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241031"
---
# <a name="add-app-to-team"></a><span data-ttu-id="4050f-103">Adicionar o aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="4050f-103">Add app to team</span></span>



<span data-ttu-id="4050f-104">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="4050f-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4050f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4050f-105">Permissions</span></span>
<span data-ttu-id="4050f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4050f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4050f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4050f-108">Permission type</span></span>      | <span data-ttu-id="4050f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4050f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4050f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4050f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4050f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4050f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4050f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4050f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4050f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4050f-113">Not supported.</span></span>    |
|<span data-ttu-id="4050f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4050f-114">Application</span></span> | <span data-ttu-id="4050f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4050f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4050f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4050f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="4050f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4050f-117">Request headers</span></span>
| <span data-ttu-id="4050f-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4050f-118">Header</span></span>       | <span data-ttu-id="4050f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="4050f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4050f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4050f-120">Authorization</span></span>  | <span data-ttu-id="4050f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4050f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4050f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4050f-123">Request body</span></span>

| <span data-ttu-id="4050f-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4050f-124">Property</span></span>     | <span data-ttu-id="4050f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="4050f-125">Type</span></span>   |<span data-ttu-id="4050f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4050f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4050f-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4050f-127">teamsApp</span></span>| [<span data-ttu-id="4050f-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4050f-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="4050f-129">Para adicionar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4050f-129">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="4050f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4050f-130">Response</span></span>

<span data-ttu-id="4050f-131">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4050f-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4050f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4050f-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4050f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4050f-133">Request</span></span>
<span data-ttu-id="4050f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4050f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST /teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="4050f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4050f-135">Response</span></span>
<span data-ttu-id="4050f-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4050f-136">The following is an example of the response.</span></span> <span data-ttu-id="4050f-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4050f-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4050f-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4050f-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="4050f-139">Veja também</span><span class="sxs-lookup"><span data-stu-id="4050f-139">See also</span></span>

