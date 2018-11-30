---
title: Obter softwareUpdateStatusSummary
description: Ler propriedades e relações do objeto softwareUpdateStatusSummary.
ms.openlocfilehash: 7dfbcbf5ce2e2424abcf2b6180548b882591d09e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040117"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="4f2ed-103">Obter softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4f2ed-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="4f2ed-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f2ed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f2ed-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f2ed-107">Ler propriedades e relações do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="4f2ed-107">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f2ed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f2ed-108">Prerequisites</span></span>
<span data-ttu-id="4f2ed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f2ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f2ed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f2ed-111">Permission type</span></span>|<span data-ttu-id="4f2ed-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f2ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f2ed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f2ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f2ed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f2ed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4f2ed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f2ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f2ed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-116">Not supported.</span></span>|
|<span data-ttu-id="4f2ed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f2ed-117">Application</span></span>|<span data-ttu-id="4f2ed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f2ed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f2ed-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f2ed-120">Optional query parameters</span></span>
<span data-ttu-id="4f2ed-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4f2ed-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2ed-122">Request headers</span></span>
|<span data-ttu-id="4f2ed-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f2ed-123">Header</span></span>|<span data-ttu-id="4f2ed-124">Valor</span><span class="sxs-lookup"><span data-stu-id="4f2ed-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f2ed-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f2ed-125">Authorization</span></span>|<span data-ttu-id="4f2ed-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f2ed-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4f2ed-127">Accept</span></span>|<span data-ttu-id="4f2ed-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4f2ed-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f2ed-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2ed-129">Request body</span></span>
<span data-ttu-id="4f2ed-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f2ed-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f2ed-131">Response</span></span>
<span data-ttu-id="4f2ed-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-132">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f2ed-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f2ed-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f2ed-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2ed-134">Request</span></span>
<span data-ttu-id="4f2ed-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="4f2ed-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f2ed-136">Response</span></span>
<span data-ttu-id="4f2ed-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f2ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





