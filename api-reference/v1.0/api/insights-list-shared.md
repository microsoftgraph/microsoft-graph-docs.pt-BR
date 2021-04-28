---
title: Listar compartilhados
description: Visão calculada que retorna a lista de arquivos compartilhados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0b799be314ce9f2519d7174c84f9349b09bbd5c3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050420"
---
# <a name="list-shared"></a><span data-ttu-id="da6e7-103">Listar compartilhados</span><span class="sxs-lookup"><span data-stu-id="da6e7-103">List shared</span></span>

<span data-ttu-id="da6e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da6e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da6e7-105">Insight calculado que inclui a lista de documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="da6e7-105">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="da6e7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="da6e7-106">Permissions</span></span>
<span data-ttu-id="da6e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da6e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da6e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da6e7-109">Permission type</span></span>      | <span data-ttu-id="da6e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da6e7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da6e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da6e7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da6e7-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da6e7-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="da6e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da6e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da6e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da6e7-114">Not supported.</span></span>    |
|<span data-ttu-id="da6e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da6e7-115">Application</span></span> | <span data-ttu-id="da6e7-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da6e7-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da6e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da6e7-117">HTTP request</span></span>
<span data-ttu-id="da6e7-118">Obter uma lista de documentos compartilhados com o usuário de assinatura.</span><span class="sxs-lookup"><span data-stu-id="da6e7-118">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="da6e7-119">**Observação**: somente o usuário pode fazer solicitações usando a ID ou o nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="da6e7-119">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="da6e7-120">Expanda o recurso referenciado por uma **visão compartilhada:**</span><span class="sxs-lookup"><span data-stu-id="da6e7-120">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da6e7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da6e7-121">Optional query parameters</span></span>
<span data-ttu-id="da6e7-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da6e7-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="da6e7-123">Você pode usar o `$filter` parâmetro de consulta para filtrar itens compartilhados.</span><span class="sxs-lookup"><span data-stu-id="da6e7-123">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="da6e7-124">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="da6e7-124">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="da6e7-125">Consulte os tipos e tipos de contêiner disponíveis que você pode filtrar em [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="da6e7-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="da6e7-126">Você também pode recuperar arquivos compartilhados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="da6e7-126">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="da6e7-127">Por exemplo, especificando a `lastshared/sharedby/address` propriedade:</span><span class="sxs-lookup"><span data-stu-id="da6e7-127">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="da6e7-128">Consulte o [tipo complexo sharingDetail.](../resources/insights-sharingdetail.md)</span><span class="sxs-lookup"><span data-stu-id="da6e7-128">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="da6e7-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da6e7-129">Request headers</span></span>
| <span data-ttu-id="da6e7-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da6e7-130">Header</span></span>       |  <span data-ttu-id="da6e7-131">Valor</span><span class="sxs-lookup"><span data-stu-id="da6e7-131">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="da6e7-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="da6e7-132">Authorization</span></span>  | <span data-ttu-id="da6e7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da6e7-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="da6e7-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da6e7-135">Accept</span></span>  | <span data-ttu-id="da6e7-136">application/json</span><span class="sxs-lookup"><span data-stu-id="da6e7-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da6e7-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da6e7-137">Request body</span></span>
<span data-ttu-id="da6e7-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da6e7-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da6e7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="da6e7-139">Response</span></span>

<span data-ttu-id="da6e7-140">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` lista de itens compartilhados no corpo da resposta. [](../resources/insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="da6e7-140">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da6e7-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da6e7-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="da6e7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da6e7-142">Request</span></span>

<span data-ttu-id="da6e7-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da6e7-143">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="da6e7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="da6e7-144">Response</span></span>

<span data-ttu-id="da6e7-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da6e7-145">Here is an example of the response.</span></span> <span data-ttu-id="da6e7-146">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da6e7-146">Note: The response object shown here might be shortened for readability.</span></span>

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
