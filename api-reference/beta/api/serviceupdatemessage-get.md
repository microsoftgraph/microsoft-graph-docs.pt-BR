---
title: Obter serviceUpdateMessage
description: Recupere as propriedades e as relações de um objeto serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 63a9342d7c1db2f8716d5f4e255e91630287ba1f
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151731"
---
# <a name="get-serviceupdatemessage"></a><span data-ttu-id="976a0-103">Obter serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="976a0-103">Get serviceUpdateMessage</span></span>
<span data-ttu-id="976a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="976a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="976a0-105">Recupere as propriedades e as relações de um [objeto serviceUpdateMessage.](../resources/serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="976a0-105">Retrieve the properties and relationships of a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object.</span></span>

<span data-ttu-id="976a0-106">Essa operação recupera uma mensagem de atualização de serviço especificada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="976a0-106">This operation retrieves a specified service update message for the tenant.</span></span> <span data-ttu-id="976a0-107">A operação retornará um erro se a mensagem não existir para o locatário.</span><span class="sxs-lookup"><span data-stu-id="976a0-107">The operation returns an error if the message does not exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="976a0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="976a0-108">Permissions</span></span>
<span data-ttu-id="976a0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="976a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="976a0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="976a0-111">Permission type</span></span>|<span data-ttu-id="976a0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="976a0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="976a0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="976a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="976a0-114">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="976a0-114">ServiceMessage.Read.All</span></span>|
|<span data-ttu-id="976a0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="976a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="976a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="976a0-116">Not supported.</span></span>|
|<span data-ttu-id="976a0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="976a0-117">Application</span></span>|<span data-ttu-id="976a0-118">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="976a0-118">ServiceMessage.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="976a0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="976a0-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages/{serviceUpdateMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="976a0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="976a0-120">Optional query parameters</span></span>
<span data-ttu-id="976a0-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="976a0-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="976a0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="976a0-122">Request headers</span></span>
|<span data-ttu-id="976a0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="976a0-123">Name</span></span>|<span data-ttu-id="976a0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="976a0-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="976a0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="976a0-125">Authorization</span></span>|<span data-ttu-id="976a0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="976a0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="976a0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="976a0-128">Request body</span></span>
<span data-ttu-id="976a0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="976a0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="976a0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="976a0-130">Response</span></span>

<span data-ttu-id="976a0-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto serviceUpdateMessage](../resources/serviceupdatemessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="976a0-131">If successful, this method returns a `200 OK` response code and a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="976a0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="976a0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="976a0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="976a0-133">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["MC172851"],
  "name": "get_serviceupdatemessage"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/MC172851
```

### <a name="response"></a><span data-ttu-id="976a0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="976a0-134">Response</span></span>
><span data-ttu-id="976a0-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="976a0-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/messages/$entity",
    "startDateTime": "2019-02-01T18:51:00Z",
    "endDateTime": "2019-06-01T08:00:00Z",
    "lastModifiedDateTime": "2021-01-08T01:10:06.843Z",
    "title": "(Updated) New feature: Changes to PowerPoint and Word to open files faster",
    "id": "MC172851",
    "category": "StayInformed",
    "severity": "Normal",
    "tags": [
      "Updated message"
    ],
    "isMajorChange": true,
    "actionRequiredByDateTime": null,
    "services": [
      "SharePoint Online",
      "OneDrive for Business"
    ],
    "details": [
      {
        "name": "ExternalLink",
        "value": "https://support.office.com/article/office-document-cache-settings-4b497318-ae4f-4a99-be42-b242b2e8b692"
      }
    ],
    "body": {
      "contentType": "Text",
      "content": "Updated January 07, 2021: Based on learnings from our early rings, we have made the decision to make additional changes to the code before we proceed with the rollout. We will update the Message center post once we re-start the rollout.  Thank you for your patience........"
    },
    "viewPoint": null
}
```