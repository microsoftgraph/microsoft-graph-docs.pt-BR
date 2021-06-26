---
title: Listar mensagens
description: Recupere os recursos serviceUpdateMessage da propriedade de navegação de mensagens.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 9aca8752be18bad686677c4c718492ea93ccf0f4
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151451"
---
# <a name="list-messages"></a><span data-ttu-id="e4e5a-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="e4e5a-103">List messages</span></span>
<span data-ttu-id="e4e5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4e5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4e5a-105">Recupere os [recursos serviceUpdateMessage](../resources/serviceupdatemessage.md) da **propriedade de navegação de** mensagens.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-105">Retrieve the [serviceUpdateMessage](../resources/serviceupdatemessage.md) resources from the **messages** navigation property.</span></span>

<span data-ttu-id="e4e5a-106">Essa operação recupera todas as mensagens de atualização de serviço existentes para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-106">This operation retrieves all service update messages that exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4e5a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4e5a-107">Permissions</span></span>
<span data-ttu-id="e4e5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4e5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e5a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4e5a-110">Permission type</span></span>|<span data-ttu-id="e4e5a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4e5a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4e5a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4e5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4e5a-113">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4e5a-113">ServiceMessage.Read.All</span></span>|
|<span data-ttu-id="e4e5a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4e5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4e5a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-115">Not supported.</span></span>|
|<span data-ttu-id="e4e5a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4e5a-116">Application</span></span>|<span data-ttu-id="e4e5a-117">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4e5a-117">ServiceMessage.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4e5a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4e5a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4e5a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e4e5a-119">Optional query parameters</span></span>
<span data-ttu-id="e4e5a-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4e5a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4e5a-121">Request headers</span></span>
|<span data-ttu-id="e4e5a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e4e5a-122">Name</span></span>|<span data-ttu-id="e4e5a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4e5a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4e5a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4e5a-124">Authorization</span></span>|<span data-ttu-id="e4e5a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4e5a-127">Request body</span></span>
<span data-ttu-id="e4e5a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4e5a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4e5a-129">Response</span></span>

<span data-ttu-id="e4e5a-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos serviceUpdateMessage](../resources/serviceupdatemessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-130">If successful, this method returns a `200 OK` response code and a collection of [serviceUpdateMessage](../resources/serviceupdatemessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e5a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4e5a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4e5a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4e5a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_serviceupdatemessage"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages
```

### <a name="response"></a><span data-ttu-id="e4e5a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4e5a-133">Response</span></span>
><span data-ttu-id="e4e5a-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/messages",
  "value": [
    {
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
        "content": "Updated January 07, 2021: Based on learnings from our early rings, we have made the decision to make additional changes to the code before we proceed with the rollout. We will update the Message center post once we re-start the rollout......"
      },
      "viewPoint": null
    }
  ]
}
```

