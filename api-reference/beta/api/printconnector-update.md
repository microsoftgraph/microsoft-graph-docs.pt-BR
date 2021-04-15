---
title: Atualizar printConnector
description: Atualize as propriedades de um objeto printConnector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ad196f179a81f9d5467ba715a08730b09ad4b88c
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766039"
---
# <a name="update-printconnector"></a><span data-ttu-id="942f7-103">Atualizar printConnector</span><span class="sxs-lookup"><span data-stu-id="942f7-103">Update printConnector</span></span>

<span data-ttu-id="942f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="942f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942f7-105">Atualize as propriedades de um **objeto printConnector.**</span><span class="sxs-lookup"><span data-stu-id="942f7-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="942f7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="942f7-106">Permissions</span></span>
<span data-ttu-id="942f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="942f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="942f7-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="942f7-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="942f7-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="942f7-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="942f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="942f7-111">Permission type</span></span> | <span data-ttu-id="942f7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="942f7-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="942f7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="942f7-113">Delegated (work or school account)</span></span>| <span data-ttu-id="942f7-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942f7-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="942f7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="942f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="942f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="942f7-116">Not Supported.</span></span>|
|<span data-ttu-id="942f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="942f7-117">Application</span></span>|<span data-ttu-id="942f7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="942f7-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="942f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="942f7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="942f7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="942f7-120">Request headers</span></span>
| <span data-ttu-id="942f7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="942f7-121">Name</span></span>       | <span data-ttu-id="942f7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="942f7-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="942f7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="942f7-123">Authorization</span></span> | <span data-ttu-id="942f7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="942f7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="942f7-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="942f7-126">Content-type</span></span>  | <span data-ttu-id="942f7-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="942f7-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="942f7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="942f7-129">Request body</span></span>
<span data-ttu-id="942f7-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="942f7-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="942f7-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="942f7-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="942f7-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="942f7-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="942f7-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="942f7-133">Property</span></span>     | <span data-ttu-id="942f7-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="942f7-134">Type</span></span>        | <span data-ttu-id="942f7-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="942f7-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="942f7-136">nome</span><span class="sxs-lookup"><span data-stu-id="942f7-136">name</span></span>|<span data-ttu-id="942f7-137">String</span><span class="sxs-lookup"><span data-stu-id="942f7-137">String</span></span>|<span data-ttu-id="942f7-138">O nome do conector.</span><span class="sxs-lookup"><span data-stu-id="942f7-138">The name of the connector.</span></span>|
|<span data-ttu-id="942f7-139">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="942f7-139">fullyQualifiedDomainName</span></span>|<span data-ttu-id="942f7-140">String</span><span class="sxs-lookup"><span data-stu-id="942f7-140">String</span></span>|<span data-ttu-id="942f7-141">O nome de host do computador do conector.</span><span class="sxs-lookup"><span data-stu-id="942f7-141">The connector machine's hostname.</span></span>|
|<span data-ttu-id="942f7-142">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="942f7-142">operatingSystem</span></span>|<span data-ttu-id="942f7-143">String</span><span class="sxs-lookup"><span data-stu-id="942f7-143">String</span></span>|<span data-ttu-id="942f7-144">A versão do sistema operacional do conector.</span><span class="sxs-lookup"><span data-stu-id="942f7-144">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="942f7-145">appVersion</span><span class="sxs-lookup"><span data-stu-id="942f7-145">appVersion</span></span>|<span data-ttu-id="942f7-146">String</span><span class="sxs-lookup"><span data-stu-id="942f7-146">String</span></span>|<span data-ttu-id="942f7-147">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="942f7-147">The connector's version.</span></span>|
|<span data-ttu-id="942f7-148">localização</span><span class="sxs-lookup"><span data-stu-id="942f7-148">location</span></span>|[<span data-ttu-id="942f7-149">printerLocation</span><span class="sxs-lookup"><span data-stu-id="942f7-149">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="942f7-150">O local físico e/ou organizacional do conector.</span><span class="sxs-lookup"><span data-stu-id="942f7-150">The physical and/or organizational location of the connector.</span></span>|

## <a name="response"></a><span data-ttu-id="942f7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="942f7-151">Response</span></span>
<span data-ttu-id="942f7-152">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printConnector](../resources/printConnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="942f7-152">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="942f7-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="942f7-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="942f7-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="942f7-154">Request</span></span>
<span data-ttu-id="942f7-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="942f7-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="942f7-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="942f7-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connector"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/connectors/{id}
Content-type: application/json
Content-length: 300

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

---

##### <a name="response"></a><span data-ttu-id="942f7-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="942f7-157">Response</span></span>
<span data-ttu-id="942f7-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="942f7-158">The following is an example of the response.</span></span>
><span data-ttu-id="942f7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="942f7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
