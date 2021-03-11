---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e as relações do objeto chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2a3fe469cd0a1cf10242c1f89370c8a6932ec866
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634283"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="55d81-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="55d81-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="55d81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55d81-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55d81-105">Recupere as propriedades e as relações do [objeto chatMessageHostedContent.](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="55d81-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55d81-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55d81-106">Permissions</span></span>

<span data-ttu-id="55d81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55d81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55d81-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55d81-109">Permission type</span></span>                        | <span data-ttu-id="55d81-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55d81-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="55d81-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55d81-111">Delegated (work or school account)</span></span>| <span data-ttu-id="55d81-112">Para **recurso de** canal: ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="55d81-112">For **channel** resource: ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="55d81-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55d81-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55d81-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55d81-114">Not supported.</span></span>|
|<span data-ttu-id="55d81-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55d81-115">Application</span></span>| <span data-ttu-id="55d81-116">Para **recurso** de canal: ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="55d81-116">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="55d81-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="55d81-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="55d81-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55d81-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="55d81-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="55d81-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="55d81-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55d81-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents/{hosted-content-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55d81-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55d81-121">Optional query parameters</span></span>

<span data-ttu-id="55d81-122">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55d81-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55d81-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55d81-123">Request headers</span></span>

| <span data-ttu-id="55d81-124">Nome</span><span class="sxs-lookup"><span data-stu-id="55d81-124">Name</span></span>      |<span data-ttu-id="55d81-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="55d81-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55d81-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="55d81-126">Authorization</span></span> | <span data-ttu-id="55d81-127">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="55d81-127">Bearer {code}.</span></span> <span data-ttu-id="55d81-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55d81-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55d81-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55d81-129">Request body</span></span>

<span data-ttu-id="55d81-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55d81-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55d81-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="55d81-131">Response</span></span>

<span data-ttu-id="55d81-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55d81-132">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55d81-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55d81-133">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="55d81-134">Exemplo 1: Obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="55d81-134">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="55d81-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55d81-135">Request</span></span>

<span data-ttu-id="55d81-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55d81-136">The following is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents/aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv
```

#### <a name="response"></a><span data-ttu-id="55d81-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="55d81-137">Response</span></span>

<span data-ttu-id="55d81-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55d81-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="55d81-139">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="55d81-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55d81-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55d81-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1614618259349')/hostedContents/$entity",
    "id": "aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-hosted-content-bytes"></a><span data-ttu-id="55d81-141">Exemplo 2: Obter bytes de conteúdo hospedados</span><span class="sxs-lookup"><span data-stu-id="55d81-141">Example 2: Get hosted content bytes</span></span>

#### <a name="request"></a><span data-ttu-id="55d81-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55d81-142">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents/aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv/$value
```

#### <a name="response"></a><span data-ttu-id="55d81-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="55d81-143">Response</span></span>

> [!NOTE]
> <span data-ttu-id="55d81-144">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="55d81-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55d81-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55d81-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201

<ContentBytes>
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


