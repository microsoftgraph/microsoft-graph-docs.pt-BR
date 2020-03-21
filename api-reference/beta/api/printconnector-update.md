---
title: Atualizar o multiligação
description: Atualiza as propriedades de um objeto Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6546693f0a158de15c6ccb2ca82829748926f16c
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895578"
---
# <a name="update-printconnector"></a><span data-ttu-id="37121-103">Atualizar o multiligação</span><span class="sxs-lookup"><span data-stu-id="37121-103">Update printConnector</span></span>

<span data-ttu-id="37121-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37121-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37121-105">Atualiza as propriedades **de um objeto** Printer.</span><span class="sxs-lookup"><span data-stu-id="37121-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37121-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37121-106">Permissions</span></span>
<span data-ttu-id="37121-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37121-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="37121-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="37121-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="37121-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37121-110">Permission type</span></span> | <span data-ttu-id="37121-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37121-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="37121-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37121-112">Delegated (work or school account)</span></span>| <span data-ttu-id="37121-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="37121-113">Users.Read.All</span></span> |
|<span data-ttu-id="37121-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37121-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37121-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37121-115">Not Supported.</span></span>|
|<span data-ttu-id="37121-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37121-116">Application</span></span>|<span data-ttu-id="37121-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37121-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37121-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37121-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="37121-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37121-119">Request headers</span></span>
| <span data-ttu-id="37121-120">Nome</span><span class="sxs-lookup"><span data-stu-id="37121-120">Name</span></span>       | <span data-ttu-id="37121-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="37121-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="37121-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="37121-122">Authorization</span></span> | <span data-ttu-id="37121-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37121-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37121-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="37121-125">Content-type</span></span>  | <span data-ttu-id="37121-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37121-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37121-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37121-128">Request body</span></span>
<span data-ttu-id="37121-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="37121-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="37121-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="37121-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="37121-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="37121-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="37121-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37121-132">Property</span></span>     | <span data-ttu-id="37121-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="37121-133">Type</span></span>        | <span data-ttu-id="37121-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="37121-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="37121-135">nome</span><span class="sxs-lookup"><span data-stu-id="37121-135">name</span></span>|<span data-ttu-id="37121-136">String</span><span class="sxs-lookup"><span data-stu-id="37121-136">String</span></span>|<span data-ttu-id="37121-137">O nome do conector.</span><span class="sxs-lookup"><span data-stu-id="37121-137">The name of the connector.</span></span>|
|<span data-ttu-id="37121-138">Nomededomíniototalmentequalificado</span><span class="sxs-lookup"><span data-stu-id="37121-138">fullyQualifiedDomainName</span></span>|<span data-ttu-id="37121-139">String</span><span class="sxs-lookup"><span data-stu-id="37121-139">String</span></span>|<span data-ttu-id="37121-140">O nome de host do computador do conector.</span><span class="sxs-lookup"><span data-stu-id="37121-140">The connector machine's hostname.</span></span>|
|<span data-ttu-id="37121-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="37121-141">operatingSystem</span></span>|<span data-ttu-id="37121-142">String</span><span class="sxs-lookup"><span data-stu-id="37121-142">String</span></span>|<span data-ttu-id="37121-143">A versão do sistema operacional do computador do conector.</span><span class="sxs-lookup"><span data-stu-id="37121-143">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="37121-144">appVersion</span><span class="sxs-lookup"><span data-stu-id="37121-144">appVersion</span></span>|<span data-ttu-id="37121-145">String</span><span class="sxs-lookup"><span data-stu-id="37121-145">String</span></span>|<span data-ttu-id="37121-146">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="37121-146">The connector's version.</span></span>|
|<span data-ttu-id="37121-147">location</span><span class="sxs-lookup"><span data-stu-id="37121-147">location</span></span>|[<span data-ttu-id="37121-148">printerLocation</span><span class="sxs-lookup"><span data-stu-id="37121-148">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="37121-149">O local físico e/ou organizacional do conector.</span><span class="sxs-lookup"><span data-stu-id="37121-149">The physical and/or organizational location of the connector.</span></span>|

## <a name="response"></a><span data-ttu-id="37121-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="37121-150">Response</span></span>
<span data-ttu-id="37121-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [multiconnect](../resources/printConnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37121-151">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37121-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37121-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37121-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37121-153">Request</span></span>
<span data-ttu-id="37121-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37121-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connector"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/connectors/{id}
Content-type: application/json
Content-length: 300

{
  "name": "ConnectorName",
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
##### <a name="response"></a><span data-ttu-id="37121-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="37121-155">Response</span></span>
<span data-ttu-id="37121-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37121-156">The following is an example of the response.</span></span>
><span data-ttu-id="37121-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37121-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 406

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "name": "ConnectorName",
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
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
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
  },
  "registeredBy": {}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->