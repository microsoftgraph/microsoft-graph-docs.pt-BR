---
title: 'cloudCommunications: getPresencesByUserId'
description: Obtenha as informações de presença de vários usuários.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: e06c1403b1d96a42a670f4c6d53c3bf5251d3b8a
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581176"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="76fbf-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="76fbf-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="76fbf-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76fbf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76fbf-105">Obtenha as informações de [presença](../resources/presence.md) de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="76fbf-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="76fbf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="76fbf-106">Permissions</span></span>
<span data-ttu-id="76fbf-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="76fbf-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="76fbf-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76fbf-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76fbf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76fbf-109">Permission type</span></span> | <span data-ttu-id="76fbf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76fbf-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="76fbf-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76fbf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="76fbf-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="76fbf-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="76fbf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76fbf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76fbf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76fbf-114">Not Supported.</span></span>                         |
| <span data-ttu-id="76fbf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76fbf-115">Application</span></span>                            | <span data-ttu-id="76fbf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76fbf-116">Not Supported.</span></span>                                  |

> <span data-ttu-id="76fbf-117">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="76fbf-117">**Note:**</span></span>
> * <span data-ttu-id="76fbf-118">O máximo de 650 IDs de usuário têm suporte por solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="76fbf-118">Maximum of 650 user IDs are supported per API request.</span></span>
> * <span data-ttu-id="76fbf-119">A taxa máxima de solicitações dessa API são 1500 solicitações de API em um período de 30 segundos, por aplicativo por locatário.</span><span class="sxs-lookup"><span data-stu-id="76fbf-119">The maximum request rate of this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="76fbf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76fbf-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="76fbf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76fbf-121">Request Headers</span></span>
| <span data-ttu-id="76fbf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="76fbf-122">Name</span></span>          | <span data-ttu-id="76fbf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="76fbf-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="76fbf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="76fbf-124">Authorization</span></span> | <span data-ttu-id="76fbf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76fbf-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="76fbf-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="76fbf-127">Content-type</span></span> | <span data-ttu-id="76fbf-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76fbf-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="76fbf-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76fbf-130">Request body</span></span>

<span data-ttu-id="76fbf-131">No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="76fbf-131">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="76fbf-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="76fbf-132">Parameter</span></span>      | <span data-ttu-id="76fbf-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="76fbf-133">Type</span></span>    |<span data-ttu-id="76fbf-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="76fbf-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76fbf-135">ids</span><span class="sxs-lookup"><span data-stu-id="76fbf-135">ids</span></span>|<span data-ttu-id="76fbf-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="76fbf-136">String collection</span></span>|<span data-ttu-id="76fbf-137">As IDs de objeto de usuário.</span><span class="sxs-lookup"><span data-stu-id="76fbf-137">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="76fbf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="76fbf-138">Response</span></span>

<span data-ttu-id="76fbf-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76fbf-139">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="76fbf-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="76fbf-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76fbf-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76fbf-141">Request</span></span>
<span data-ttu-id="76fbf-142">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="76fbf-142">The following example shows a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```

---

### <a name="response"></a><span data-ttu-id="76fbf-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="76fbf-143">Response</span></span>
<span data-ttu-id="76fbf-144">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="76fbf-144">The following example shows the response.</span></span>

> <span data-ttu-id="76fbf-145">**Observação:** Os objetos Response podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="76fbf-145">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="76fbf-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76fbf-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get-presence-multiple-users",
  "truncated": "true",
  "@odata.type": "microsoft.graph.presence"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574
```
```json
{
    "value": [{
            "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
            "availability": "Busy",
            "activity": "InAMeeting"
        },
        {
            "id": "66825e03-7ef5-42da-9069-724602c31f6b",
            "availability": "Away",
            "activity": "Away"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Presence Information",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


