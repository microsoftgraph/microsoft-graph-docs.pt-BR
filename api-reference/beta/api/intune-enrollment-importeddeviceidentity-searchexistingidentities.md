---
title: Ação searchExistingIdentities
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b33ea0e3e70771c6567e0b507fa1ce04dcbf8741
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228053"
---
# <a name="searchexistingidentities-action"></a><span data-ttu-id="90132-103">Ação searchExistingIdentities</span><span class="sxs-lookup"><span data-stu-id="90132-103">searchExistingIdentities action</span></span>

<span data-ttu-id="90132-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90132-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90132-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90132-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90132-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90132-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90132-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="90132-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90132-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90132-108">Prerequisites</span></span>
<span data-ttu-id="90132-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90132-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90132-111">Permission type</span></span>|<span data-ttu-id="90132-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90132-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90132-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90132-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90132-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="90132-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="90132-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90132-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90132-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90132-116">Not supported.</span></span>|
|<span data-ttu-id="90132-117">Application</span><span class="sxs-lookup"><span data-stu-id="90132-117">Application</span></span>|<span data-ttu-id="90132-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="90132-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90132-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90132-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/searchExistingIdentities
```

## <a name="request-headers"></a><span data-ttu-id="90132-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90132-120">Request headers</span></span>
|<span data-ttu-id="90132-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90132-121">Header</span></span>|<span data-ttu-id="90132-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90132-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90132-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90132-123">Authorization</span></span>|<span data-ttu-id="90132-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90132-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90132-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90132-125">Accept</span></span>|<span data-ttu-id="90132-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90132-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90132-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90132-127">Request body</span></span>
<span data-ttu-id="90132-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="90132-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="90132-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="90132-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="90132-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90132-130">Property</span></span>|<span data-ttu-id="90132-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90132-131">Type</span></span>|<span data-ttu-id="90132-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90132-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90132-133">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="90132-133">importedDeviceIdentities</span></span>|<span data-ttu-id="90132-134">coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="90132-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="90132-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="90132-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="90132-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="90132-136">Response</span></span>
<span data-ttu-id="90132-137">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90132-137">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90132-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90132-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="90132-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90132-139">Request</span></span>
<span data-ttu-id="90132-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90132-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/searchExistingIdentities

Content-type: application/json
Content-length: 596

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="90132-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="90132-141">Response</span></span>
<span data-ttu-id="90132-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90132-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```




