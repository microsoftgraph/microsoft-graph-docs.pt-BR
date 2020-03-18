---
title: Ação importDeviceIdentityList
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9a7128b4d49137cf722b5556c64049049c8d190
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42805211"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="478eb-103">Ação importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="478eb-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="478eb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="478eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="478eb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="478eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="478eb-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="478eb-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="478eb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="478eb-107">Prerequisites</span></span>
<span data-ttu-id="478eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="478eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="478eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="478eb-110">Permission type</span></span>|<span data-ttu-id="478eb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="478eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="478eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="478eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="478eb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="478eb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="478eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="478eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="478eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="478eb-115">Not supported.</span></span>|
|<span data-ttu-id="478eb-116">Application</span><span class="sxs-lookup"><span data-stu-id="478eb-116">Application</span></span>|<span data-ttu-id="478eb-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="478eb-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="478eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="478eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="478eb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="478eb-119">Request headers</span></span>
|<span data-ttu-id="478eb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="478eb-120">Header</span></span>|<span data-ttu-id="478eb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="478eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="478eb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="478eb-122">Authorization</span></span>|<span data-ttu-id="478eb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="478eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="478eb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="478eb-124">Accept</span></span>|<span data-ttu-id="478eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="478eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="478eb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="478eb-126">Request body</span></span>
<span data-ttu-id="478eb-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="478eb-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="478eb-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="478eb-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="478eb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="478eb-129">Property</span></span>|<span data-ttu-id="478eb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="478eb-130">Type</span></span>|<span data-ttu-id="478eb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="478eb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="478eb-132">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="478eb-132">importedDeviceIdentities</span></span>|<span data-ttu-id="478eb-133">coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="478eb-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="478eb-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="478eb-134">Not yet documented</span></span>|
|<span data-ttu-id="478eb-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="478eb-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="478eb-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="478eb-136">Boolean</span></span>|<span data-ttu-id="478eb-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="478eb-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="478eb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="478eb-138">Response</span></span>
<span data-ttu-id="478eb-139">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="478eb-139">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="478eb-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="478eb-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="478eb-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="478eb-141">Request</span></span>
<span data-ttu-id="478eb-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="478eb-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

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
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="478eb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="478eb-143">Response</span></span>
<span data-ttu-id="478eb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="478eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```




