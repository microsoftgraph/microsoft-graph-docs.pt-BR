---
title: Listar compartilhados
description: Visão calculada que retorna a lista de arquivos compartilhados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 6a02e149f830dffe2795b3fbb6477005797e0adc
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473238"
---
# <a name="list-shared"></a><span data-ttu-id="fab27-103">Listar compartilhados</span><span class="sxs-lookup"><span data-stu-id="fab27-103">List shared</span></span>

<span data-ttu-id="fab27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fab27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fab27-105">Insight calculado que inclui a lista de documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="fab27-105">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fab27-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fab27-106">Permissions</span></span>
<span data-ttu-id="fab27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fab27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fab27-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fab27-109">Permission type</span></span>      | <span data-ttu-id="fab27-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fab27-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fab27-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fab27-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fab27-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fab27-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fab27-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fab27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fab27-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fab27-114">Not supported.</span></span>    |
|<span data-ttu-id="fab27-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fab27-115">Application</span></span> | <span data-ttu-id="fab27-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fab27-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fab27-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fab27-117">HTTP request</span></span>
<span data-ttu-id="fab27-118">Obter uma lista de documentos compartilhados com o usuário de assinatura.</span><span class="sxs-lookup"><span data-stu-id="fab27-118">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="fab27-119">**Observação**: somente o usuário pode fazer solicitações usando a ID ou o nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="fab27-119">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="fab27-120">Expanda o recurso referenciado por uma **visão compartilhada:**</span><span class="sxs-lookup"><span data-stu-id="fab27-120">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fab27-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fab27-121">Optional query parameters</span></span>
<span data-ttu-id="fab27-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fab27-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="fab27-123">Você pode usar o `$filter` parâmetro de consulta para filtrar itens compartilhados.</span><span class="sxs-lookup"><span data-stu-id="fab27-123">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="fab27-124">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="fab27-124">For example, based on **type**:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="fab27-125">Consulte os tipos e tipos de contêiner disponíveis que você pode filtrar em [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="fab27-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="fab27-126">Você também pode recuperar arquivos compartilhados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="fab27-126">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="fab27-127">Por exemplo, especificando a `lastshared/sharedby/address` propriedade:</span><span class="sxs-lookup"><span data-stu-id="fab27-127">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="fab27-128">Consulte o [tipo complexo sharingDetail.](../resources/insights-sharingdetail.md)</span><span class="sxs-lookup"><span data-stu-id="fab27-128">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="fab27-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fab27-129">Request headers</span></span>
| <span data-ttu-id="fab27-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fab27-130">Header</span></span>       |  <span data-ttu-id="fab27-131">Valor</span><span class="sxs-lookup"><span data-stu-id="fab27-131">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="fab27-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="fab27-132">Authorization</span></span>  | <span data-ttu-id="fab27-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fab27-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="fab27-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fab27-135">Accept</span></span>  | <span data-ttu-id="fab27-136">application/json</span><span class="sxs-lookup"><span data-stu-id="fab27-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fab27-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fab27-137">Request body</span></span>
<span data-ttu-id="fab27-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fab27-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fab27-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab27-139">Response</span></span>

<span data-ttu-id="fab27-140">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` lista de itens compartilhados no corpo da resposta. [](../resources/insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="fab27-140">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fab27-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fab27-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fab27-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fab27-142">Request</span></span>

<span data-ttu-id="fab27-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fab27-143">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

### <a name="response"></a><span data-ttu-id="fab27-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab27-144">Response</span></span>

<span data-ttu-id="fab27-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fab27-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "AWb0Qy4TEA1KhLW-k1L5mSjtxZAcxDFkTKiTNA-2kZDTXzrMX_4FhECOU0bKZVj1uReivYoYYoJNqTeuC-x1Agtm9EMuExANSoS1vpNS-ZkoBA",
            "lastShared": {
                "sharedDateTime": "2021-03-23T08:41:05Z",
                "sharingType": "Direct",
                "sharedBy": {
                    "displayName": "Megan Bowen",
                    "address": "MeganB@contoso.com",
                    "id": "3e0c9f05-b9b8-4cf5-9b35-a4e11b24b5b7"
                },
                "sharingReference": {}
            },
            "resourceVisualization": {
                "title": "CE Annual Report",
                "type": "Word",
                "mediaType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
                "previewImageUrl": "https://contoso-my.sharepoint.com/_api/v2.0/drives/b!ZvRDLhMQDUqEtb6TUvmZKO3FkBzEMWRMqJM0D7aRkNNfOsxf_gWEQI5TRsplWPW5/items/01K6ZMU4QXUK6YUGDCQJG2SN5OBPWHKAQL/thumbnails/0/small/thumbnailContent",
                "previewText": "Contoso Annual Report Anne Wallace Sales Contoso today announced financial results for its most recent fi",
                "containerWebUrl": "https://contoso-my.sharepoint.com/personal/meganb_m365x841051_onmicrosoft_com/Documents/Forms/All.aspx",
                "containerDisplayName": "Megan Bowen",
                "containerType": "OneDriveBusiness"
            },
            "resourceReference": {
                "webUrl": "https://contoso-my.sharepoint.com/personal/meganb_m365x841051_onmicrosoft_com/_layouts/15/Doc.aspx?sourcedoc=%7B8ABDA217-6218-4D82-A937-AE0BEC75020B%7D&file=CE%20Annual%20Report.docx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!ZvRDLhMQDUqEtb6TUvmZKO3FkBzEMWRMqJM0D7aRkNNfOsxf_gWEQI5TRsplWPW5/items/01K6ZMU4QXUK6YUGDCQJG2SN5OBPWHKAQL",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```
