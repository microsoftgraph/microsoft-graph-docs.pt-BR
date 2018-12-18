---
title: Obter softwareUpdateStatusSummary
description: Ler propriedades e relações do objeto softwareUpdateStatusSummary.
author: tfitzmac
ms.openlocfilehash: 4f490db4042c03233f2613e44b6a6f90460f9345
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354023"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="d5bd8-103">Obter softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d5bd8-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="d5bd8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5bd8-105">Ler propriedades e relações do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="d5bd8-105">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5bd8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5bd8-106">Prerequisites</span></span>
<span data-ttu-id="d5bd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5bd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5bd8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5bd8-109">Permission type</span></span>|<span data-ttu-id="d5bd8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5bd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5bd8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5bd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5bd8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5bd8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d5bd8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5bd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5bd8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-114">Not supported.</span></span>|
|<span data-ttu-id="d5bd8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5bd8-115">Application</span></span>|<span data-ttu-id="d5bd8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5bd8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5bd8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5bd8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d5bd8-118">Optional query parameters</span></span>
<span data-ttu-id="d5bd8-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d5bd8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bd8-120">Request headers</span></span>
|<span data-ttu-id="d5bd8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5bd8-121">Header</span></span>|<span data-ttu-id="d5bd8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d5bd8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5bd8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5bd8-123">Authorization</span></span>|<span data-ttu-id="d5bd8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5bd8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5bd8-125">Accept</span></span>|<span data-ttu-id="d5bd8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5bd8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5bd8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bd8-127">Request body</span></span>
<span data-ttu-id="d5bd8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5bd8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bd8-129">Response</span></span>
<span data-ttu-id="d5bd8-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-130">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5bd8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5bd8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5bd8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bd8-132">Request</span></span>
<span data-ttu-id="d5bd8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="d5bd8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bd8-134">Response</span></span>
<span data-ttu-id="d5bd8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5bd8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```



