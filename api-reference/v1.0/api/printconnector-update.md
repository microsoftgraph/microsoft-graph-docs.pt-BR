---
title: Atualizar printConnector
description: Atualize as propriedades de um objeto printConnector.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1fea6a1fe18012dcca1c266304e4430b1adcd660
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516844"
---
# <a name="update-printconnector"></a><span data-ttu-id="a8a41-103">Atualizar printConnector</span><span class="sxs-lookup"><span data-stu-id="a8a41-103">Update printConnector</span></span>
<span data-ttu-id="a8a41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8a41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a8a41-105">Atualize as propriedades de um **objeto printConnector.**</span><span class="sxs-lookup"><span data-stu-id="a8a41-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8a41-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8a41-106">Permissions</span></span>
<span data-ttu-id="a8a41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8a41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a8a41-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8a41-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a8a41-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a8a41-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a8a41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8a41-111">Permission type</span></span> | <span data-ttu-id="a8a41-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8a41-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a8a41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8a41-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a8a41-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8a41-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="a8a41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8a41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8a41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8a41-116">Not Supported.</span></span>|
|<span data-ttu-id="a8a41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8a41-117">Application</span></span>|<span data-ttu-id="a8a41-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8a41-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8a41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8a41-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="a8a41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a41-120">Request headers</span></span>
|<span data-ttu-id="a8a41-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a8a41-121">Name</span></span>|<span data-ttu-id="a8a41-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8a41-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a8a41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8a41-123">Authorization</span></span>|<span data-ttu-id="a8a41-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8a41-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a8a41-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8a41-126">Content-Type</span></span>|<span data-ttu-id="a8a41-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8a41-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8a41-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a41-129">Request body</span></span>
<span data-ttu-id="a8a41-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a8a41-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a8a41-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a8a41-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a8a41-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a8a41-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a8a41-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8a41-133">Response</span></span>
<span data-ttu-id="a8a41-134">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printConnector](../resources/printConnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8a41-134">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8a41-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8a41-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8a41-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a41-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printconnector"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
Content-Type: application/json
Content-length: 308

{
  "displayName": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```


### <a name="response"></a><span data-ttu-id="a8a41-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8a41-137">Response</span></span>
<span data-ttu-id="a8a41-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8a41-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "displayName": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```

