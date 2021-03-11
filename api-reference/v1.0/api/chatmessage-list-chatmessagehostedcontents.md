---
title: Listar chatMessageHostedContents
description: Recupere a lista de objetos chatMessageHostedContent de uma mensagem.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16dc59427eeab168d816780c9fcdc5c6603a1955
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634284"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="382aa-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="382aa-103">List hostedContents</span></span>

<span data-ttu-id="382aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="382aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="382aa-105">Recupere a lista de [objetos chatMessageHostedContent](../resources/chatmessagehostedcontent.md) de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="382aa-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="382aa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="382aa-106">Permissions</span></span>

<span data-ttu-id="382aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="382aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="382aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="382aa-109">Permission type</span></span>                        | <span data-ttu-id="382aa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="382aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="382aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="382aa-111">Delegated (work or school account)</span></span>| <span data-ttu-id="382aa-112">Para **recurso de** canal: ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="382aa-112">For **channel** resource: ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="382aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="382aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="382aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="382aa-114">Not supported.</span></span>|
|<span data-ttu-id="382aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="382aa-115">Application</span></span>| <span data-ttu-id="382aa-116">Para **recurso** de canal: ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="382aa-116">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="382aa-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="382aa-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="382aa-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="382aa-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="382aa-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="382aa-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="382aa-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="382aa-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="382aa-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="382aa-121">Optional query parameters</span></span>

<span data-ttu-id="382aa-122">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="382aa-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="382aa-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="382aa-123">Request headers</span></span>

| <span data-ttu-id="382aa-124">Nome</span><span class="sxs-lookup"><span data-stu-id="382aa-124">Name</span></span>      |<span data-ttu-id="382aa-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="382aa-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="382aa-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="382aa-126">Authorization</span></span> | <span data-ttu-id="382aa-127">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="382aa-127">Bearer {code}.</span></span> <span data-ttu-id="382aa-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="382aa-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="382aa-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="382aa-129">Request body</span></span>

<span data-ttu-id="382aa-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="382aa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="382aa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="382aa-131">Response</span></span>

<span data-ttu-id="382aa-132">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="382aa-132">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="382aa-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="382aa-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="382aa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="382aa-134">Request</span></span>

<span data-ttu-id="382aa-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="382aa-135">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents
```

### <a name="response"></a><span data-ttu-id="382aa-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="382aa-136">Response</span></span>

<span data-ttu-id="382aa-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="382aa-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="382aa-138">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="382aa-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="382aa-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="382aa-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1614618259349')/hostedContents",
    "@odata.count": 1,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


