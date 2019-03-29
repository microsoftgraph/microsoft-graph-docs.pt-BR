---
title: Obter windowsInformationProtectionWipeAction
description: Leia as propriedades e as relações do objeto windowsInformationProtectionWipeAction.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad145cccf75ffad4abf8a939306e178440118b49
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977566"
---
# <a name="get-windowsinformationprotectionwipeaction"></a><span data-ttu-id="dd352-103">Obter windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="dd352-103">Get windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="dd352-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd352-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd352-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd352-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd352-106">Leia as propriedades e as relações do objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="dd352-106">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd352-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd352-107">Prerequisites</span></span>
<span data-ttu-id="dd352-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd352-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd352-110">Permission type</span></span>|<span data-ttu-id="dd352-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd352-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd352-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd352-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd352-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd352-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dd352-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd352-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd352-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd352-115">Not supported.</span></span>|
|<span data-ttu-id="dd352-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd352-116">Application</span></span>|<span data-ttu-id="dd352-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd352-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd352-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd352-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd352-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dd352-119">Optional query parameters</span></span>
<span data-ttu-id="dd352-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dd352-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd352-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd352-121">Request headers</span></span>
|<span data-ttu-id="dd352-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd352-122">Header</span></span>|<span data-ttu-id="dd352-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dd352-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd352-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd352-124">Authorization</span></span>|<span data-ttu-id="dd352-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd352-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd352-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd352-126">Accept</span></span>|<span data-ttu-id="dd352-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dd352-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd352-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd352-128">Request body</span></span>
<span data-ttu-id="dd352-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd352-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd352-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd352-130">Response</span></span>
<span data-ttu-id="dd352-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd352-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd352-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd352-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd352-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd352-133">Request</span></span>
<span data-ttu-id="dd352-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd352-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

### <a name="response"></a><span data-ttu-id="dd352-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd352-135">Response</span></span>
<span data-ttu-id="dd352-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd352-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
    "id": "2620a996-a996-2620-96a9-202696a92026",
    "status": "pending",
    "targetedUserId": "Targeted User Id value",
    "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
    "targetedDeviceName": "Targeted Device Name value",
    "targetedDeviceMacAddress": "Targeted Device Mac Address value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
  }
}
```




