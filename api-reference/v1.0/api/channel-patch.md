---
title: Canal de patch
description: Atualiza as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b90e3abff3d0624b7639195f02e342f7fa11c5ee
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848924"
---
# <a name="patch-channel"></a><span data-ttu-id="3ecd5-103">Canal de patch</span><span class="sxs-lookup"><span data-stu-id="3ecd5-103">Patch channel</span></span>

<span data-ttu-id="3ecd5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ecd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ecd5-105">Atualiza as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ecd5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ecd5-106">Permissions</span></span>

<span data-ttu-id="3ecd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ecd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ecd5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ecd5-109">Permission type</span></span>      | <span data-ttu-id="3ecd5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ecd5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ecd5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ecd5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ecd5-112">ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3ecd5-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3ecd5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ecd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ecd5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-114">Not supported.</span></span>    |
|<span data-ttu-id="3ecd5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ecd5-115">Application</span></span> | <span data-ttu-id="3ecd5-116">ChannelSettings. ReadWrite. Group \*, ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3ecd5-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="3ecd5-117">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-117">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="3ecd5-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3ecd5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ecd5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3ecd5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ecd5-120">Request headers</span></span>
| <span data-ttu-id="3ecd5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ecd5-121">Header</span></span>       | <span data-ttu-id="3ecd5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3ecd5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ecd5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ecd5-123">Authorization</span></span>  | <span data-ttu-id="3ecd5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3ecd5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ecd5-126">Content-Type</span></span>  | <span data-ttu-id="3ecd5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3ecd5-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ecd5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ecd5-128">Request body</span></span>

<span data-ttu-id="3ecd5-129">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="3ecd5-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="3ecd5-130">**Observação:** Não é possível atualizar o `membershipType` valor de um canal existente.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-130">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="3ecd5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ecd5-131">Response</span></span>

<span data-ttu-id="3ecd5-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3ecd5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ecd5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ecd5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ecd5-134">Request</span></span>

<span data-ttu-id="3ecd5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-135">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```

<!-- {
  "blockType": "request",
  "name": "update_channel"
}-->

### <a name="response"></a><span data-ttu-id="3ecd5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ecd5-136">Response</span></span>

<span data-ttu-id="3ecd5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ecd5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
